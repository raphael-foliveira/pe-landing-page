<script>
	import MasterclassGradient from '$lib/components/masterclass/MasterclassGradient.svelte';
	import Modules from '$lib/components/certif-content/Modules.svelte';
	import SuccessGuide from './SuccessGuide.svelte';
</script>

<div class="background mx-2 lg:p-12 rounded-3xl flex flex-wrap my-8">
	<div class="flex justify-between w-full lg:mx-14">
		<div class="mx-auto lg:mx-0">
			<button class="btn bg-white rounded-3xl lg:p-10 font-black">CONTEÚDO DA CERTIFICAÇÃO</button>
		</div>
		<div class="lg:flex content-middle hidden">
			<MasterclassGradient color="black" />
		</div>
	</div>
	<div class="flex flex-wrap lg:justify-around">
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
