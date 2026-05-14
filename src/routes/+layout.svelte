<script lang="ts">
	import '../app.css';
	import Header from '../components/header.svelte';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={'/favicon.ico'} />
	<title>Regis N. - Software Engineer</title>
</svelte:head>

<main class="overflow-y-hidden bg-amber-100/10 h-screen">
	<Header />

	{@render children?.()}
</main>
