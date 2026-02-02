<script lang="ts">
	type SectionProps = {
		title: string;
		subTitle?: string;
		items: (
			| string
			| {
					content: string;
					subItems?: string[];
			  }
		)[];
	};

	const { title, subTitle, items }: SectionProps = $props();
</script>

<div class="m-2 flex flex-col gap-2">
	<h4 class="flex justify-center rounded-4xl border-2 px-4 py-2">{title.toUpperCase()}</h4>
	{#if subTitle}
		<h6 class="flex justify-center">{subTitle}</h6>
	{/if}
	<ul class="mx-8 flex list-disc flex-col">
		{#each items as item, index (index)}
			<li>
				{#if typeof item === "string"}
					{item}
				{:else}
					<!-- eslint-disable-next-line svelte/no-at-html-tags -->
					{@html item.content}
					{#if item.subItems?.length}
						<ul class="mx-8 flex list-[circle] flex-col">
							{#each item.subItems as subItem, subIndex (subIndex)}
								<li>{subItem}</li>
							{/each}
						</ul>
					{/if}
				{/if}
			</li>
		{/each}
	</ul>
</div>
