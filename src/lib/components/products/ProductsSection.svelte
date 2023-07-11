<script>
	import MasterclassGradient from '../masterclass/MasterclassGradient.svelte';
	import ProductPictures from './ProductPictures.svelte';
</script>

<div class="lg:px-32 py-8 lg:py-20 flex justify-center flex-wrap">
	<MasterclassGradient />

	<div class="products-card w-full rounded-3xl p-4 lg:p-12 flex mt-8 lg:mt-32">
		<div class="w-full lg:w-1/2 flex flex-wrap">
			<p class="text-xl lg:text-3xl text-center lg:text-left w-full">
				<strong>Veja alguns dos produtos que você terá em seu portfólio,</strong> para atender os mais
				diversos perfis de clientes.
			</p>
			<ul class="text-xl lg:text-2xl mt-auto list-disc px-4">
				<li>Programa de Distensionamento de Coluna</li>
				<li>Programa de Realinhamento da Patela</li>
				<li>Programa de Saúde para Gestante</li>
				<li>Programa de Saúde para Diabéticos</li>
				<li>Programa de Saúde para Hipertenso</li>
				<li>Programa de Saúde para Esteatose Hepática</li>
				<li>Programa de Saúde para Obesidade e Sobrepeso</li>
				<li>Programa de Hipertrofia</li>
				<li>Programa de Redução de Celulite - Glúteo Max</li>
			</ul>
		</div>
		<div class="hidden lg:flex w-full z-40 top-24">
			<div class="w-2/3 ml-auto mr-60 flex flex-wrap flex-row-reverse relative bottom-48">
				<ProductPictures />
			</div>
		</div>
	</div>
</div>
<div class="lg:h-96" />
<div class="flex justify-center lg:p-16 lg:mt-48">
	<button class="py-4 px-4 lg:px-20 rounded-3xl font-black text-xl lg:text-4xl"
		>GARANTA SUA VAGA!</button
	>
</div>

<style>
	.products-card {
		background-color: var(--color-background);
		max-height: 700px;
	}
	li {
		margin: 0.5rem 0;
	}
	button {
		background-color: #00f583;
		color: #003252;
	}
</style>
