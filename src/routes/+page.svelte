<script lang="ts">
	import Card from '$lib/Card.svelte';
	import GridContainer from '$lib/GridContainer.svelte';
	import Whats from '$lib/icons/Whats.svelte';
</script>

<div class="container mx-auto mb-10 px-4">
	<h1 class="text-3xl">Lotes ubicados en San Bernardino, Horquetas de Sarapiquí</h1>
</div>

<GridContainer>
	<Card
		href="/planos/671580_inscripcion.pdf"
		price={6200000}
		area={410}
		title="Lote frente a calle pública"
	/>
	<Card
		href="planos/671585_inscripcion.pdf"
		price={6200000}
		area={410}
		title="Lote frente a calle pública"
	/>
	<Card
		href="planos/671581_inscripcion.pdf"
		price={6000000}
		area={410}
		title="Lote frente a servidumbre"
	/>
	<Card
		href="planos/671582_inscripcion.pdf"
		price={6000000}
		area={404}
		title="Lote frente a servidumbre"
	/>
	<Card
		href="planos/671589_inscripcion.pdf"
		price={6000000}
		area={410}
		title="Lote frente a servidumbre"
	/>
	<Card
		href="planos/671592_inscripcion.pdf"
		price={6000000}
		area={408}
		title="Lote frente a servidumbre"
	/>
	<Card
		href="planos/671596_inscripcion.pdf"
		price={7500000}
		area={560}
		title="Lote frente a servidumbre"
	/>
	<Card
		href="planos/671598_inscripcion.pdf"
		price={6600000}
		area={485}
		title="Lote frente a servidumbre"
		note="** Los 838 metros del plano incluyen la servidumbre. El área aprovechable es 485 metros"
	/>
</GridContainer>

<div class="container mx-auto mt-20 px-2">
	<h2 class="text-3xl my-10">Datos generales de los lotes</h2>
	<a href="https://wa.me/50689066157" target="_blank" class="text-lg link hover:link-secondary"
		><Whats />Para contactarme por Whatsapp clickea acá</a
	>
	<iframe
		src="https://www.google.com/maps/embed?pb=!1m17!1m12!1m3!1d3926.244595734181!2d-83.88922932302123!3d10.241846455134445!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m2!1m1!2zMTDCsDE0JzMxLjAiTiA4M8KwNTMnMTYuNSJX!5e0!3m2!1sen!2scr!4v1692660336248!5m2!1sen!2scr"
		class="border-none w-full h-[50vh] mt-10 mx-auto"
		allowfullscreen={true}
		loading="lazy"
		referrerpolicy="no-referrer-when-downgrade"
		title="Ubicacion de los lotes"
	/>
</div>
