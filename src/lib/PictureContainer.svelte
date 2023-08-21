<script lang="ts">
	export let src: string;
	let open = false;
	const uuid = crypto.randomUUID();

	function showModal() {
		const dialogElement = document.getElementById(uuid) as HTMLDialogElement;
		if (dialogElement) {
			dialogElement.showModal();
		}
	}
</script>

<button class="btn h-fit" on:click={showModal}
	><img {src} alt="Propiedad en San Bernardino" /></button
>
<dialog id={uuid} class="modal">
	<form method="dialog" class="modal-box max-w-5xl">
		<button class="btn btn-sm btn-circle btn-ghost absolute right-2 top-2">✕</button>
		<img {src} alt="Propiedad en San Bernardino" class="mt-4" />
	</form>
</dialog>
