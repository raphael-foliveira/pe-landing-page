<script>
	import MasterclassGradient from './MasterclassGradient.svelte';
	import GradientContainer from '../containers/GradientContainer.svelte';
</script>

<GradientContainer>
	<div class="h-screen p-28 pb-52 w-full flex flex-wrap">
		<MasterclassGradient />
		<div class="flex flex-wrap right-border h-auto w-1/2 h-full pr-20 pt-12">
			<p class="text-white text-6xl font-black leading-normal">
				Você tem algum desses problemas no seu dia dia como Personal Trainer?
			</p>
		</div>
		<div class="w-1/2 text-white text-3xl pl-12 border-solid">
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

	.text-container p {
		margin: 2.5rem 0;
	}
</style>
