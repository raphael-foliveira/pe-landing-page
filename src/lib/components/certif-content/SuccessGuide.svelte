<script>
	import GuidePicture from '$lib/img/guide/guide_picture.png';
	import GradientCard from '../containers/GradientCard.svelte';
</script>

<GradientCard>
	<div class="w-1/2">
		<img src={GuidePicture} alt="" />
	</div>
	<div class="w-1/2">
		<h3 class="text-5xl">GUIA DO PERSONAL DE SUCESSO.</h3>
		<p class="text-3xl">
			Eu sei que muito profissionais não tem habilidade com vendas e aquisição de novos clientes,
			mas isso não será um problema para você.
		</p>
		<p class="text-3xl">
			Com o guia do Personal de Sucesso você vai aprender como se posicionar no mercado, captar
			clientes, vender, cobrar e conduzir os seus programa do inicio ao fim...
		</p>
		<p class="text-3xl">
			Principalmente, você vai aprender as técnicas para vender seus programas pelo valor de mais de
			R$3.000 e alavancar seus ganhos rapidamente.
		</p>
		<p class="text-3xl">
			Essa é grande novidade que colocamos na Certificação do Método Customizado, para você faturar
			de 10 a 20 mil reais todos os meses.
		</p>
	</div>
</GradientCard>

<style>
	p {
		margin: 3rem 0;
	}
</style>
