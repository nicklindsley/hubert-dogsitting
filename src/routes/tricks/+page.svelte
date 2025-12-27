<script lang="ts">
	import type { ComponentProps } from 'svelte';
	import { digging } from '$lib/assets/trickVideos';
	import TrickVideo from '$lib/components/TrickVideo.svelte';

	const trickVideos: ComponentProps<typeof TrickVideo>['video'][] = [
		{
			title: 'Sit',
			verbalCue: 'Sit',
			handCue: 'Hold your fist out about waist high',
			url: digging,
		},
		{
			title: 'Shake',
			verbalCue: 'Shake',
			handCue: 'Hold your palm out in front of his right paw',
			url: undefined,
		},
		{
			title: 'Other Paw',
			description: 'Shake with his other paw',
			verbalCue: 'Paw',
			handCue: 'Hold your palm out in front of his left paw',
			url: undefined,
		},
		{
			title: 'High Five',
			verbalCue: 'High Five',
			handCue: 'Hold your palm verticle in front of his head',
			url: undefined,
		},
		{
			title: 'Wave',
			verbalCue: 'Wave',
			handCue:
				'Wave semi close to him. For some reason he recognizes it more if you use your left hand',
			url: undefined,
		},
		{
			title: 'Lay Down',
			verbalCue: 'Down',
			handCue: 'Tab the ground with your index finger OR tab you foot',
			url: undefined,
		},
		{
			title: 'Crawl',
			verbalCue: 'Crawl',
			handCue: 'While laying down, drag your index finger or foot across the ground',
			url: undefined,
		},
		{
			title: 'Spin',
			description: 'Spin in a circle',
			verbalCue: 'Turn',
			handCue: 'Make a clockwise circle above his head with your finger',
			url: undefined,
		},
		{
			title: 'Recall',
			description: 'Get him to come to you',
			verbalCue: 'Come',
			handCue: 'Snap your finger and point down to the ground in front of you',
			url: undefined,
		},
		{
			title: 'Touch',
			description: 'Get him to touch your finger',
			verbalCue: 'Touch',
			handCue: 'Hold your finger out horizontally',
			url: undefined,
		},
		{
			title: 'Drop It',
			description: 'Drop a toy, bone, etc',
			verbalCue: 'Drop It',
			handCue: 'Hold a closed fist below his mouth',
			url: undefined,
		},
		{
			title: 'Wait',
			description: 'Sit and wait without moving or following',
			verbalCue: 'Wait',
			handCue: 'Swipe your open hand across your body',
			url: undefined,
		},
		{
			title: 'Place',
			description: 'Go to his bed and wait',
			verbalCue: 'Place',
			handCue: 'Pound your left chest with your fist twice',
			url: undefined,
		},
		{
			title: 'Free',
			description: 'Releases him from a wait or place command',
			verbalCue: 'Free',
			handCue: "Swipe your index finger away from him (he doesn't get this one) ",
			url: undefined,
		},
		{
			title: 'Figure 8',
			description: 'Walk between your legs',
			verbalCue: 'Weave',
			handCue: 'Move your right hand behind your back',
			url: undefined,
		},
		{
			title: 'Cross Arms',
			description: 'Cross his arms over each other',
			verbalCue: 'Cross',
			handCue: 'While laying down, hold your hand out to his left',
			url: undefined,
		},
		{
			title: 'Roll Over',
			verbalCue: 'Roll',
			handCue: 'While laying down, swing your hand counter clockwise around his head',
			url: undefined,
		},
		{
			title: 'Focus',
			description: 'Look at you and maintain eye contact (helpful for pictures)',
			verbalCue: 'Focus',
			handCue: 'Tap the temple of your head',
			url: undefined,
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
