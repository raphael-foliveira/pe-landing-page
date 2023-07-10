<script>
	import MasterclassGradient from '../MasterclassGradient/MasterclassGradient.svelte';
	import Modules from './Modules.svelte';
</script>

<div class="background mx-2 p-12 rounded-3xl flex flex-wrap">
	<div class="flex justify-between w-full">
		<div>
			<button class="btn bg-white rounded-3xl p-10 font-black">CONTEÚDO DA CERTIFICAÇÃO</button>
		</div>
		<div class="flex content-middle">
			<MasterclassGradient color="black" />
		</div>
	</div>
	<Modules />
</div>

<style>
	.background {
		background-color: #f0f2fa;
	}
	button {
		color: #0097f5;
	}
</style>
