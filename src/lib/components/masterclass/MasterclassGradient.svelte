<script lang="ts">
	import LogoWhite from '$lib/img/LogoWhite.png';
	import LogoBlack from '$lib/img/LogoBlack.png';
	export let color: 'white' | 'black' = 'white';
</script>

<div class="gradient flex justify-center lg:justify-normal text-center content-center w-full">
	<p class="mr-2 align-middle lg:mt-2 text-sm lg:text-2xl">-Masterclass Personal de Sucesso</p>
	{#if color == 'white'}
		<img src={LogoWhite} alt="" class="object-cover h-4 lg:h-10 w-auto" />
	{:else}
		<img src={LogoBlack} alt="" class="object-cover h-4 lg:h-10 w-auto" />
	{/if}
</div>

<style>
	.gradient {
		text-align: center;
		font-size: 25px;
		font-weight: 800;
	}

	.gradient p {
		background: -webkit-linear-gradient(180deg, #00256d, #001cac, #009bff);
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
	}
</style>
