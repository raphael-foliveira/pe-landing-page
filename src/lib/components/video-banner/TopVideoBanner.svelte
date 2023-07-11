<script lang="ts">
	import Subscribe from '$lib/img/header/subscribe.png';
	import PLAY from '$lib/img/header/PLAY.png';
	import VideoPlayer from './VideoPlayer.svelte';
	import { onMount } from 'svelte';

	export let showVideo = false;
	let cw: number;
	$: galloBgClass = cw < 1000 ? 'bg-gallo-mobile' : 'bg-gallo';
	$: bannerContainer = cw < 1000 ? 'banner-container-mobile' : 'banner-container';

	const toggleVideo = () => {
		showVideo = !showVideo;
	};
</script>

<VideoPlayer {toggleVideo} {showVideo} />
<div class="{bannerContainer} relative" bind:clientWidth={cw}>
	<div
		class="left-10 w-full h-full bg-no-repeat flex flex-wrap p-2 lg:p-12 text-center lg:text-left"
	>
		<div class="w-full lg:w-1/2 h-full flex flex-wrap content-between">
			<div class="text-container w-full mt-24 lg:pr-40 flex flex-wrap content-around">
				<p class="text-3xl w-full font-black lg:font-normal">A metodologia de trabalho para você</p>
				<p class=" text-3xl lg:text-5xl font-black w-full">
					Ganhar 5 a 10X MAIS que o modelo de hora aula
				</p>
				<p class="text-3xl w-full">
					E faturar de 10 a 20 mil reais por mês atuando como Personal Trainer
				</p>
			</div>
			<div class="mb-4 py-8 lg:py-0">
				<a href="/">
					<img src={Subscribe} alt="" />
				</a>
			</div>
			<div class="mobile-video w-full flex lg:hidden justify-center">
				<iframe
					class="my-auto"
					width="320"
					height="160"
					src="https://www.youtube.com/embed/LpnMhSIEqfA?controls=0"
					title="YouTube video player"
					frameborder="0"
					allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
					allowfullscreen
				/>
			</div>
		</div>

		<div class="w-1/2 h-full hidden lg:flex flex-wrap justify-center content-center">
			<button on:click={toggleVideo}>
				<img src={PLAY} alt="Botão play" />
			</button>
		</div>
	</div>
	<div class="-z-50 absolute top-0 right-0 bg-right h-full w-full {galloBgClass} bg-repeat" />
</div>

<style>
	.text-container {
		color: white;
	}

	.text-container p {
		margin: 1rem 0;
		line-height: 1.4;
	}

	.banner-container {
		height: 705px;
	}
	.banner-container-mobile {
		padding-bottom: 2rem;
	}

	.bg-gallo {
		background-image: url('$lib/img/header/banner_sem_botao_2.png');
	}
	.bg-gallo-mobile {
		background-image: url('$lib/img/header/banner_mobile_1.png');
	}
</style>
