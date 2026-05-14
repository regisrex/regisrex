<script>
	import Container from '../../layouts/container.svelte';
	import imigongoSvg from '../../vectors/imigongo.svg';

	const caseStudies = [
		{
			title: 'Welcome',
			slug: 'welcome',
			date: '2024-10-17',
			excerpt: 'An introduction to my blog and what I build'
		}
		// Add your case studies here
	];
</script>

<Container className="py-10 flex flex-col gap-8">
	<div class="flex flex-col gap-4">
		<h1 class="text-4xl font-bold">Blog</h1>
		<p class="max-w-2xl text-gray-500">
			Documenting my journey building projects, solving problems, and learning along the way.
		</p>
		<div
			class="mt-2 h-10 w-full"
			style="background-image: url({imigongoSvg}); background-size: contain; background-repeat: repeat-x;"
		></div>
	</div>

	<!-- Case Studies Section -->
	<section class="flex flex-col gap-4">
		<div class="flex items-baseline gap-3">
			<h2 class="text-2xl font-bold">Case Studies</h2>
			<span class="text-sm text-gray-500">{caseStudies.length} posts</span>
		</div>
		<!-- <p class="text-gray-500">Deep dives into projects I've built from start to finish.</p> -->
		<div class="mt-4 flex flex-col gap-6">
			{#each caseStudies as post}
				<a
					href="/blogs/{post.slug}"
					class="group flex flex-col gap-1 border-l-2 border-slate-700 pl-4 transition-all hover:border-slate-400"
				>
					<div class="flex items-baseline gap-1">
						<h3 class="text-md font-semibold group-hover:text-slate-300">{post.title}</h3>
						<span class="text-sm text-gray-500">{post.date}</span>
					</div>
					<p class="text-gray-500">{post.excerpt}</p>
				</a>
			{:else}
				<p class="text-gray-500">No case studies yet. Stay tuned!</p>
			{/each}
		</div>
	</section>

</Container>
