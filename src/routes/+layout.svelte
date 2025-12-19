<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/hubert-favicon.png';
	import NavBar from '$lib/components/NavBar.svelte';

	const { children } = $props();

	const navBarLinks = [
		{ label: 'Home', route: '/' },
		{ label: 'Tricks', route: '/tricks' },
	];
</script>

<svelte:head>
	<title>Hubert Dogsitting Guide</title>
	<meta property="og:image" content={favicon} />
	<meta property="og:image:width" content="580" />
	<meta property="og:image:height" content="580" />
	<link rel="icon" href={favicon} />
</svelte:head>
<NavBar links={navBarLinks} />
{@render children()}
