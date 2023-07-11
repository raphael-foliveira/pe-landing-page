<script lang="ts">
	import MasterclassGradient from './MasterclassGradient.svelte';
	import GradientContainer from '../containers/GradientContainer.svelte';

	let cw: number;
	$: borderClass = cw > 1024 ? 'right-border' : 'bottom-border';
</script>

<GradientContainer>
	<div class="p-2 lg:p-28 w-full flex flex-wrap text-center lg:text-left" bind:clientWidth={cw}>
		<MasterclassGradient />
		<div class="flex flex-wrap w-full lg:w-1/2 h-full px-4 lg:pr-20 pt-12">
			<p
				class="text-white {borderClass} lg:text-left text-2xl lg:text-6xl font-black leading-normal"
			>
				Você tem algum desses problemas no seu dia dia como Personal Trainer?
			</p>
		</div>
		<div class="w-full lg:w-1/2 text-white text-lg lg:text-3xl px-6 lg:pl-12 lg:pr-0 border-solid">
			<div class="m-auto text-container">
				<p>
					<strong> Insegurança e falta de metodologia</strong> para garantir o resultado do seu aluno.
				</p>
				<p>
					<strong>Cobrar barato pelo seu serviço de Personal,</strong> para não perder clientes que não
					valorizam o seu trabalho.
				</p>
				<p>
					<strong>Trabalha muito, ganha pouco </strong> e não enxerga perspectiva de futuro na profissão.
				</p>
				<p>
					<strong>Impotência e descaso </strong>comparado a outros profissionais da área de saúde.
				</p>
				<p>
					<strong>Pensa em desistir da profissão </strong>e trabalhar em outra área por falta de
					reconhecimento e valorização.
				</p>
			</div>
		</div>
	</div>
</GradientContainer>

<style>
	.right-border {
		border-right: 7px solid #069eff;
	}

	.bottom-border {
		padding-bottom: 2rem;
		border-bottom: 5px solid #069eff;
	}

	.text-container p {
		margin: 2.5rem 0;
	}
</style>
