<script>
	import ProgramCard from './ProgramCard.svelte';
	import WorkToolCard from './WorkToolCard.svelte';
	import Mentoria1 from '$lib/img/product/mentoria_1.png';
	import Mentoria2 from '$lib/img/product/mentoria_2.png';
	import WhatYouGet from './WhatYouGet.svelte';
</script>

<div class="bg-white p-8">
	<WorkToolCard />
	<ProgramCard title="programa de mentoria em grupo" image={Mentoria1}>
		<p>
			A Certificação contempla um programa de mentoria em grupo, para te guiar nos seus primeiros
			passos dentro da metodologia e direcionar o seu progresso.
		</p>
		<p>
			Acompanhamento ao vivo para te ajudar a se posicionar no mercado, captar novos clientes e
			vender os seus primeiros programas.
		</p>
		<p>O QUE VOCÊ VAI APRENDER NA MENTORIA:</p>
		<ul class="list-disc ml-6">
			<li>Como atrair e captar clientes.</li>
			<li>Como vender seus primeiros programas nos primeiros 30 dias.</li>
			<li>Como fazer o fechamento de vendas dos programas.</li>
			<li>Como conduzir os programas após o fechamento.</li>
			<li>Como conduzir seus atendimentos online.</li>
			<li>Como precificar e definir os valores dos programas.</li>
		</ul>
		<p>E muito mais</p>
	</ProgramCard>
	<ProgramCard title="comunidade de alunos no facebook" image={Mentoria2}>
		<p>A comunidade representa a FAMÍLIA Gallo Personal Systems.</p>
		<p>
			A família Gallo, é um grupo seleto de profissionais de alto nível, mas também de pessoas do
			bem, para você poder tirar todas as suas dúvidas e interagir com outros profissionais que já
			estão tendo sucesso com a nossa metodologia.
		</p>
	</ProgramCard>
	<WhatYouGet />
</div>

<style>
	p,
	li {
		margin: 2rem 0;
		font-size: 1.5rem;
	}
</style>
