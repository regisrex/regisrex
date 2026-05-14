<script>
	import github from '../icons/github.svg';
	import instagram from '../icons/instagram.svg';
	import linkedin from '../icons/linkedin.svg';
	import Container from '../layouts/container.svelte';
	import imigongoSvg from '../vectors/imigongo.svg';
</script>

<Container className="py-10  flex flex-col gap-4">
	<h1 class="max-w-3xl text-4xl font-bold">Regis N<span class="text-yellow-400">.</span> <br /></h1>
	<p class="max-w-2xl text-gray-800">
		Yo, nice to see you around, my name is Regis or you can call me Rex.
	</p>

	<p class="max-w-2xl text-gray-800">
		I'm fullstack software engineer, whether it's about system design, backend, looks and ux design,
		I always find myself in the conversation. It's probably a bad thing I'm told... but I've always enjoyed it
		:lol
	</p>

	<p class="max-w-2xl text-gray-800">
		I'm currently working at <a href="https://kwikkoders.com" class="text-slate-800 italic">
			Global Kwik Koders</a
		> where I contribute to the ideating, designing and building of load-heavy, fast and accessible web applications.
	</p>

	<p class="max-w-2xl text-gray-800">
		I'm currently interested in Data Science and Interaction Design, If you love talking about any
		of the two, <a href="tel:+250788927469" class="italic opacity-80">
			let's share some quesadillas one day :)
		</a> !
	</p>

	<div class="flex items-center gap-4">
		<a href="https://github.com/regisrex">
			<img src={github} alt="GitHub" class="h-6 w-6 text-slate-500" />
		</a>
		<a href="https://instagram.com/regissrex">
			<img src={instagram} alt="Instagram" class="h-6 w-6 text-slate-500" />
		</a>
		<a href="/">
			<img src={linkedin} alt="LinkedIn" class="h-7 w-7 text-slate-500" />
		</a>
	</div>

	<div
		class="mt-6 h-10 w-full"
		style="background-image: url({imigongoSvg}); background-size: contain; background-repeat: repeat-x;"
	></div>

	<p class="text-slate-800 opacity-80 text-xs">
		© 2026 <a href="https://regiis.dev" class="underline">Regis N.</a> Powered by
		<a href="svelte.dev/docs/kit" class="underline"> SvelteKit</a>
	</p>
</Container>
