<script>
	import '../app.css';

	const year = new Date().getFullYear();
</script>

<div class="navbar bg-base-300 mb-10">
	<p class="normal-case text-xl ml-10 flex mx-auto">Rids.land</p>
	<nav class="mr-10">
		<a class="btn btn-ghost normal-case text-xl" href="/fotos">Fotos</a>
		<a class="btn btn-ghost normal-case text-xl" href="/">Planos</a>
	</nav>
</div>

<slot />

<footer class="footer footer-center p-4 bg-base-300 text-base-content mt-10">
	<div>
		<p>Copyright © {year} - Creado por José Martín Acosta</p>
	</div>
</footer>
