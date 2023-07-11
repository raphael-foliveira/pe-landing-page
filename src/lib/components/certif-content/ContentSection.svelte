<script>
	import MasterclassGradient from '$lib/components/Masterclass/MasterclassGradient.svelte';
	import Modules from '$lib/components/certif-content/Modules.svelte';
	import SuccessGuide from './SuccessGuide.svelte';
</script>

<div class="background mx-2 p-12 rounded-3xl flex flex-wrap my-8">
	<div class="flex justify-between w-full mx-14">
		<div>
			<button class="btn bg-white rounded-3xl p-10 font-black">CONTEÚDO DA CERTIFICAÇÃO</button>
		</div>
		<div class="flex content-middle">
			<MasterclassGradient color="black" />
		</div>
	</div>
	<div class="flex flex-wrap justify-around">
		<Modules />
	</div>
	<SuccessGuide />
</div>

<style>
	.background {
		background-color: #f0f2fa;
	}
	button {
		color: #0097f5;
	}
</style>
