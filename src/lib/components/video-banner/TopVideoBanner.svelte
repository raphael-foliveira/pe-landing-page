<script lang="ts">
	import Subscribe from '$lib/img/header/subscribe.png';
	import PLAY from '$lib/img/header/PLAY.png';
	import VideoPlayer from './VideoPlayer.svelte';

	export let showVideo = false;

	const toggleVideo = () => {
		showVideo = !showVideo;
	};
</script>

<VideoPlayer {toggleVideo} {showVideo} />
<div class="banner-container relative">
	<div class="left-10 w-full h-full bg-no-repeat flex flex-wrap p-12">
		<div class="w-1/2 h-full flex flex-wrap content-between">
			<div class="text-container w-full mt-24 pr-40 flex flex-wrap content-around">
				<p class="text-3xl w-full">A metodologia de trabalho para você</p>
				<p class="text-5xl font-black w-full">Ganhar 5 a 10X MAIS que o modelo de hora aula</p>
				<p class="text-3xl w-full">
					E faturar de 10 a 20 mil reais por mês atuando como Personal Trainer
				</p>
			</div>
			<div class="mb-4">
				<a href="/">
					<img src={Subscribe} alt="" />
				</a>
			</div>
		</div>

		<div class="w-1/2 h-full flex flex-wrap justify-center content-center">
			<button on:click={toggleVideo}>
				<img src={PLAY} alt="Botão play" />
			</button>
		</div>
	</div>
	<div class="-z-50 absolute top-0 right-0 bg-right h-full w-full bg-gallo bg-repeat" />
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

	.bg-gallo {
		background-image: url('$lib/img/header/banner_sem_botao_2.png');
	}
</style>
