<script lang="ts">
	type Video = {
		title: string;
		description?: string;
		verbalCue?: string;
		handCue?: string;
		url?: string;
	};

	type TrickVideoProps = {
		video: Video;
		width?: number;
	};

	const { video, width }: TrickVideoProps = $props();
</script>

<div class="border-rounded m-2 flex flex-col gap-2 rounded-2xl border-2 p-2.5">
	<h5>{video.title}</h5>
	{#if video.description}
		<p>{video.description}</p>
	{/if}
	<div class="grid grid-cols-[auto_auto] rounded border">
		{#if video.verbalCue}
			<p class="border-r border-b p-1 font-bold">Verbal Cue</p>
			<p class="border-b p-1">{video.verbalCue}</p>
		{/if}
		{#if video.handCue}
			<p class="border-r p-1 font-bold">Hand Cue</p>
			<p class="p-1">{video.handCue}</p>
		{/if}
	</div>
	{#if video.url}
		<div class="flex justify-center">
			<video class="rounded-xl" controls {width} loop>
				<source src={video.url} />
			</video>
		</div>
	{/if}
</div>
