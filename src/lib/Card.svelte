<script lang="ts">
	import AreaIcon from '$lib/icons/AreaIcon.svelte';
	import Money from '$lib/icons/Money.svelte';

	export let title: string = 'Lote frente a calle';
	export let area: number = 410;
	export let price: number = 6000000;
	export let href: string;
	export let note: string = '';

	$: formattedPrice = price.toLocaleString();
</script>

<div class="card w-80 sm:w-96 bg-base-100 shadow-xl mx-auto">
	<div class="card-body">
		<h2 class="card-title text-3xl my-6">{title}</h2>
		<p class="text-lg"><AreaIcon /><span class="font-bold">Area:</span> {area} metros cuadrados</p>
		<p class="mt-4"><Money /><span class="font-bold">&#8353; </span>{formattedPrice}</p>
		{#if note}
			<p class="text-md mt-2">{note}</p>
		{/if}
		<div class="card-actions justify-end">
			<a class="btn btn-primary" target="_blank" {href}>Ver plano</a>
		</div>
	</div>
</div>
