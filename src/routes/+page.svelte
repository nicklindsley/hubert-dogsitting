<script>
	import { hubertSleeping, hubertDigging } from '$lib/assets';
</script>

<div class="flex flex-col items-center gap-4">
	<div class="flex flex-col items-center">
		<h1 class="font-bold">Hubert Dogsitting Guide</h1>
		<p>Hubbie is a good boy</p>
		<p class="text-xs italic">...Except when he gets a pee-paw</p>
	</div>
	<img src={hubertSleeping} alt="Hubert sleeping" width={400} />
	<video controls width={200}>
		<source src={hubertDigging} />
	</video>
</div>
