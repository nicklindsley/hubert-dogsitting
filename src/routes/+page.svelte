<script>
	import { hubertSleeping, hubertDigging } from '$lib/assets';
</script>

<div class="flex flex-col items-center">
	<h1>Hubert Dogsitting Guide</h1>
	<p>Hubbie is a good boy yes he is</p>
	<img src={hubertSleeping} alt="Hubert sleeping" width={400} />
	<video controls width={200}>
		<source src={hubertDigging} />
	</video>
</div>
