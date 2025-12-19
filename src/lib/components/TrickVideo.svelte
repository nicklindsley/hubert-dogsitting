<script lang="ts">
	import { digging } from '$lib/assets/trickVideos';

	type Video = { title: string; description?: string; url: string };

	const videos = {
		digging: {
			title: 'Digging',
			description: 'Hubbie likes to dig to make his bed',
			url: digging,
		},
	} as const satisfies Record<string, Video>;
	type VideoIds = keyof typeof videos;

	type TrickVideoProps = {
		videoId: VideoIds;
		width?: number;
	};

	const { videoId, width = 200 }: TrickVideoProps = $props();

	const video = $derived(videos[videoId]);
</script>

<div>
	<video controls {width}>
		<source src={video.url} />
	</video>
</div>
