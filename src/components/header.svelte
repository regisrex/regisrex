<script>
	import github from '../icons/github.svg';
	import instagram from '../icons/instagram.svg';
	import linkedin from '../icons/linkedin.svg';
	import Container from '../layouts/container.svelte';
</script>

<Container className="flex justify-between items-center py-4">
	<div class="flex items-center gap-4">
		<img src="https://github.com/regisrex.png" alt="Logo" class="h-14 w-14 rounded-full" />
		<div class="flex flex-col">
			<p class="text-lg font-bold">R&eacute;gis N.</p>
			<p class="text-sm text-gray-500">Engineering & Product design</p>
		</div>
	</div>
	<div class="flex items-center gap-4">
		<a href="/">
			<img src={github} alt="GitHub" class="h-6 w-6 text-slate-500" />
		</a>
		<a href="/">
			<img src={instagram} alt="Instagram" class="h-6 w-6 text-slate-500" />
		</a>
		<a href="/">
			<img src={linkedin} alt="LinkedIn" class="h-6 w-6 text-slate-500" />
		</a>
	</div>
</Container>
