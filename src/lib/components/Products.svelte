<script>
	import MasterclassGradient from './MasterclassGradient/MasterclassGradient.svelte';
	import ProductPictures from './containers/ProductPictures.svelte';
</script>

<div class="px-32 py-20 flex justify-center flex-wrap">
	<MasterclassGradient />

	<div class="products-card w-full rounded-3xl p-12 flex mt-32">
		<div class="w-1/2 flex flex-wrap">
			<p class="text-3xl">
				<strong>Veja alguns dos produtos que você terá em seu portfólio,</strong> para atender os mais
				diversos perfis de clientes.
			</p>
			<ul class="text-2xl mt-auto">
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
		<div class="w-full z-40 top-24">
			<div class="w-2/3 ml-auto mr-60 flex flex-wrap flex-row-reverse relative bottom-48">
				<ProductPictures />
			</div>
		</div>
	</div>
</div>
<div class="h-96" />
<div class="flex justify-center p-16 mt-48">
	<button class="py-4 px-20 rounded-3xl font-black text-4xl">GARANTA SUA VAGA!</button>
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
