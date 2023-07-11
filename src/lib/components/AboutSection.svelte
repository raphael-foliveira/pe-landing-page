<script>
	import MasterclassGradient from './MasterclassGradient/MasterclassGradient.svelte';
	import LearningPoints from './learning-points/LearningPoints.svelte';
</script>

<div class="background">
	<div class="p-32 w-3/5 py-4">
		<div class="top-text-container h-fit text-4xl pl-6 my-12">
			<p>
				<strong> Se você disse sim a qualquer um desses itens, </strong>
				então a Certificação no Método Customizado é para você.
			</p>
		</div>

		<div class="about-container pl-6">
			<h4 class="text-3xl mb-4">Sobre a certificação</h4>
			<p class="text-2xl">
				A Certificação é o mais completo curso de capacitação, atualização e especialização prática
				e avançada em Personal Trainer que existe no mundo e reune os 3 pilares essenciais que
				sustentam uma carreira de sucesso atuando como Personal Trainer.
			</p>
		</div>
	</div>

	<LearningPoints />
	<div class="px-36 py-10">
		<MasterclassGradient color="black" />
	</div>
</div>

<style>
	.top-text-container {
		border-left: 7px solid #069eff;
	}
	.background {
		background-color: var(--color-background);
	}
</style>
