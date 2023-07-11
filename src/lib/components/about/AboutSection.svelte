<script lang="ts">
	import MasterclassGradient from '../masterclass/MasterclassGradient.svelte';
	import LearningPoints from '../learning-points/LearningPoints.svelte';

	let cw: number;
	$: borderClass = cw > 1024 ? 'top-text-container' : '';
</script>

<div class="background" bind:clientWidth={cw}>
	<div class="py-8 lg:p-32 lg:py-20 w-full lg:w-3/5 text-center lg:text-left">
		<div class="{borderClass} h-fit text-xl lg:text-4xl pl-6 lg:my-12">
			<p>
				<strong> Se você disse sim a qualquer um desses itens, </strong>
				então a Certificação no Método Customizado é para você.
			</p>
		</div>

		<div class="px-4 lg:pl-6 lg:pr-0">
			<h4 class="text-3xl lg:mb-4 font-bold lg:font-normal my-8">Sobre a certificação</h4>
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
