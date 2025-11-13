<script>
	import Container from '../layouts/container.svelte';

	const navItems = [
		{
			label: 'Blogs',
			href: '#blogs'
		},
		{
			label: 'Case studies',
			href: '#case-studies'
		},
		{
			label: 'About',
			href: '#about'
		},
		{
			label: 'Contact',
			href: '#contact'
		}
	];
</script>

<Container className="flex py-4 items-center border-b border-slate-200 gap-4">
	{#each navItems as item}
		<a href={item.href} class=" text-gray-500">{item.label}</a>
	{/each}
</Container>
