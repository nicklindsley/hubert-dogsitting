<script lang="ts">
	import type { ComponentProps } from 'svelte';
	import * as TrickVideos from '$lib/assets/trickVideos';
	import TrickVideo from '$lib/components/TrickVideo.svelte';

	const trickVideos: ComponentProps<typeof TrickVideo>['video'][] = [
		{
			title: 'Sit',
			verbalCue: 'Sit',
			handCue: 'Hold your fist out about waist high',
			url: TrickVideos.sit,
		},
		{
			title: 'Shake',
			verbalCue: 'Shake',
			handCue: 'Hold your palm out in front of his right paw',
			url: TrickVideos.shake,
		},
		{
			title: 'Other Paw',
			description: 'Shake with his other paw',
			verbalCue: 'Paw',
			handCue: 'Hold your palm out in front of his left paw',
			url: TrickVideos.paw,
		},
		{
			title: 'High Five',
			verbalCue: 'High Five',
			handCue: 'Hold your palm verticle in front of his head',
			url: TrickVideos.highFive,
		},
		{
			title: 'Wave',
			verbalCue: 'Wave',
			handCue:
				'Wave semi close to him. For some reason he recognizes it more if you use your left hand',
			url: TrickVideos.wave,
		},
		{
			title: 'Lay Down',
			verbalCue: 'Down',
			handCue: 'Tab the ground with your index finger OR tab you foot',
			url: TrickVideos.down,
		},
		{
			title: 'Crawl',
			verbalCue: 'Crawl',
			handCue: 'While laying down, drag your index finger or foot across the ground',
			url: TrickVideos.crawl,
		},
		{
			title: 'Spin',
			description: 'Spin in a circle',
			verbalCue: 'Turn',
			handCue: 'Make a clockwise circle above his head with your finger',
			url: TrickVideos.turn,
		},
		{
			title: 'Recall',
			description: 'Get him to come to you',
			verbalCue: 'Come',
			handCue: 'Snap your finger and point down to the ground in front of you',
		},
		{
			title: 'Touch',
			description: 'Get him to touch your finger',
			verbalCue: 'Touch',
			handCue: 'Hold your finger out horizontally',
			url: TrickVideos.touch,
		},
		{
			title: 'Drop It',
			description: 'Drop a toy, bone, etc',
			verbalCue: 'Drop It',
			handCue: 'Hold a closed fist below his mouth',
		},
		{
			title: 'Wait',
			description: 'Sit and wait without moving or following',
			verbalCue: 'Wait',
			handCue: 'Swipe your open hand across your body',
			url: TrickVideos.wait,
		},
		{
			title: 'Place',
			description: 'Go to his bed and wait',
			verbalCue: 'Place',
			handCue: 'Pound your left chest with your fist twice',
			url: TrickVideos.place,
		},
		{
			title: 'Free',
			description: 'Releases him from a wait or place command',
			verbalCue: 'Free',
			handCue: "Swipe your index finger away from him (he doesn't get this one) ",
		},
		{
			title: 'Figure 8',
			description: 'Walk between your legs',
			verbalCue: 'Weave',
			handCue: 'Move your right hand behind your back',
			url: TrickVideos.weave,
		},
		{
			title: 'Peek',
			description: 'Poke his head under your arm',
			verbalCue: 'Peek',
			handCue:
				'Hold your left arm out horizontally, let him jump up, and hold your right finger below your left arm',
			url: TrickVideos.peek,
		},
		{
			title: 'Roll Over',
			verbalCue: 'Roll',
			handCue: 'While laying down, swing your hand counter clockwise around his head',
			url: TrickVideos.roll,
		},
		{
			title: 'Focus',
			description: 'Look at you and maintain eye contact (helpful for pictures)',
			verbalCue: 'Focus',
			handCue: 'Tap the temple of your head',
		},
	];
</script>

<div>
	<div class="grid grid-cols-3 gap-5">
		{#each trickVideos as video (video.title)}
			<TrickVideo {video} />
		{/each}
	</div>
</div>
