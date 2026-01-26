<script lang="ts">
	type SectionProps = {
		title: string;
		items: {
			content: string;
			subItems?: string[];
		}[];
	};

	const { title, items }: SectionProps = $props();
</script>

<div class="m-2 flex flex-col gap-2">
	<h5 class="flex justify-center rounded-4xl border-2 px-4 py-2">{title.toUpperCase()}</h5>
	<ul class="mx-8 flex list-disc flex-col">
		{#each items as item, index (index)}
			<li>
				<!-- eslint-disable-next-line svelte/no-at-html-tags -->
				{@html item.content}
				{#if item.subItems?.length}
					<ul class="mx-8 flex list-[circle] flex-col">
						{#each item.subItems as subItem, subIndex (subIndex)}
							<li>{subItem}</li>
						{/each}
					</ul>
				{/if}
			</li>
		{/each}
	</ul>
</div>
