<script lang="ts">
	import { page } from '$app/state';
	import { resolve } from '$app/paths';
	import type { RouteId } from '$app/types';

	const currentRoute = $derived(page.route.id);

	type NavBarProps = {
		links?: { label: string; route: RouteId }[];
	};

	const { links = [] }: NavBarProps = $props();
</script>

<div class="sticky top-0 flex min-h-10 w-full flex-col items-center bg-orange-200">
	<h3>Hubert Dogsitting Guide</h3>
	<div class="flex gap-5">
		{#each links as link (link.label)}
			<h6>
				<a
					class={`hover:underline ${currentRoute === link.route ? 'font-bold' : ''}`}
					href={resolve(link.route)}
				>
					{link.label}
				</a>
			</h6>
		{/each}
	</div>
</div>
