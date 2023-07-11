<script lang="ts">
	import IconPhoto from '$lib/img/product/what_you_get/icon__Photo_Video_.png';
	import IconMobile from '$lib/img/product/what_you_get/icon__mobile_browser_.png';
	import IconFilm from '$lib/img/product/what_you_get/icon__film_.png';
	import IconMovie from '$lib/img/product/what_you_get/icon__movie_play_.png';
	import IconPlay from '$lib/img/product/what_you_get//icon__play_circle_.png';
	import IconVideo from '$lib/img/product/what_you_get/icon__video_.png';
	import Goodie from './Goodie.svelte';

	const goodies = [
		{ image: IconPhoto, text: 'Mais de 50 aulas gravadas todas voltadas para sua prática.' },
		{
			image: IconPlay,
			text: 'Assista quantas vezes quiser por 2 anos'
		},
		{
			image: IconMobile,
			text: 'Assista no computador, tablet ou celular.'
		},
		{
			image: IconFilm,
			text: 'Vídeos com qualidade cinematográfica.'
		},
		{
			image: IconMovie,
			text: 'Conteúdo dividido em 08 módulos.'
		}
	];
</script>

<div class="rounded-3xl p-8 flex flex-wrap card justify-center">
	<h3 class="text-3xl w-full my-8">O QUE VOCÊ RECEBE AO SE INSCREVER NA CERTIFICAÇÃO</h3>
	<div class="flex flex-wrap justify-around">
		{#each goodies as goodie}
			<Goodie {...goodie} />
		{/each}
	</div>
</div>

<style>
	h3 {
		background: linear-gradient(0deg, #003252 0%, #0097f5 100%);
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
		background-clip: text;
		color: transparent;
	}
	div.card {
		background-color: #f8f8f8;
	}
</style>
