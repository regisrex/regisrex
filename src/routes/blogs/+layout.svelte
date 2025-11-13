<script>
	import Container from '../../layouts/container.svelte';
	let { children } = $props();
</script>

<Container className="py-10">
	{@render children?.()}
</Container>
