<script lang="ts">
	import type { ComponentProps } from 'svelte';
	import Video from '$lib/components/Video.svelte';
	import { digging } from '$lib/assets/trickVideos';

	const trickVideos: ComponentProps<typeof Video>['video'][] = [
		{
			title: 'Sit',
			description: 'Hold your fist out about waist high and say "sit"',
			url: digging,
		},
	];
</script>

<div>
	<div class="grid grid-cols-3 gap-5">
		{#each trickVideos as video (video.title)}
			<Video {video} />
		{/each}
	</div>
</div>
