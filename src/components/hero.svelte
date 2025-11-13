<script>
	import Container from '../layouts/container.svelte';
	import imigongoSvg from '../vectors/imigongo.svg';
</script>

<Container className="py-10  flex flex-col gap-4">
	<h1 class="max-w-3xl text-4xl font-bold">Regis N. <br> 
	<span class="text-sm font-mono text-slate-300">./regis.log</span></h1>
	<p class="max-w-2xl text-gray-500">
		Currently I'm working as a fullstack software engineer and product designer.
	</p>

	<p class="max-w-2xl text-gray-500">
		I'm currently working as an software engineer <a
			href="https://kwikkoders.com"
			class="text-slate-400">@kwikkoders</a
		>
		where I'm responsible for building and maintaining web applications.
	</p>

	<div
		class="mt-6 h-10 w-full"
		style="background-image: url({imigongoSvg}); background-size: contain; background-repeat: repeat-x;"
	></div>
	<p class="max-w-2xl text-gray-500">
		I'm gonna be sharing case studies and how I engineer. <br />
		Stay tuned.
	</p>
</Container>
