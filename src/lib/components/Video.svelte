<script lang="ts">
	type Video = { title: string; description?: string; url: string };

	type VideoProps = {
		video: Video;
		width?: number;
	};

	const { video, width = 200 }: VideoProps = $props();
</script>

<div class="border-rounded m-2 flex flex-col gap-2 rounded-2xl border p-2.5">
	<h6>{video.title}</h6>
	{#if video.description}
		<p>{video.description}</p>
	{/if}
	<div class="flex justify-center">
		<video controls {width}>
			<source src={video.url} />
		</video>
	</div>
</div>
