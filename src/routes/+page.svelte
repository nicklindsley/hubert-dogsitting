<script lang="ts">
	import { hubertSleeping } from '$lib/assets';
	import TrickVideo from '$lib/components/TrickVideo.svelte';
</script>

<div class="flex flex-col items-center gap-4">
	<div class="flex flex-col items-center">
		<h1>Hubert Dogsitting Guide</h1>
		<p>Hubbie is a good boy</p>
		<p class="text-xs italic">...Except when he gets a pee-paw</p>
	</div>
	<img src={hubertSleeping} alt="Hubert sleeping" width={400} />
	<TrickVideo videoId="digging" />
</div>
