<script lang="ts">
	import LogoWhite from '$lib/img/LogoWhite.png';
	import LogoBlack from '$lib/img/LogoBlack.png';
	export let color: 'white' | 'black' = 'white';
</script>

<div class="gradient flex text-center content-center w-full h-40">
	<p class="mr-2 align-middle mt-2">-Masterclass Personal de Sucesso</p>
	{#if color == 'white'}
		<img src={LogoWhite} alt="" class="h-10 w-auto" />
	{:else}
		<img src={LogoBlack} alt="" class="h-10 w-auto" />
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
