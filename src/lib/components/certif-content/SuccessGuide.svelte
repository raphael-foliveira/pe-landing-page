<script>
	import GuidePicture from '$lib/img/guide/guide_picture.png';
	import GradientCard from '../containers/GradientCard.svelte';
</script>

<GradientCard>
	<div class="w-full lg:w-1/2 mb-4">
		<img src={GuidePicture} alt="" />
	</div>
	<div class="w-full lg:w-1/2 text-xl text-center lg:text-left lg:text-3xl">
		<h3 class="text-xl text-center lg:text-5xl lg:text-left">GUIA DO PERSONAL DE SUCESSO.</h3>
		<p>
			Eu sei que muito profissionais não tem habilidade com vendas e aquisição de novos clientes,
			mas isso não será um problema para você.
		</p>
		<p>
			Com o guia do Personal de Sucesso você vai aprender como se posicionar no mercado, captar
			clientes, vender, cobrar e conduzir os seus programa do inicio ao fim...
		</p>
		<p>
			Principalmente, você vai aprender as técnicas para vender seus programas pelo valor de mais de
			R$3.000 e alavancar seus ganhos rapidamente.
		</p>
		<p>
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
