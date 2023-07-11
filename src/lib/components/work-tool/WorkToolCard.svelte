<script>
	import Computer from '$lib/img/product/computer.png';
	import SystemDemo from '$lib/img/product/system_demo.png';
	import MasterclassGradient from '../Masterclass/MasterclassGradient.svelte';
</script>

<div class="rounded-3xl p-8 text-white flex flex-wrap card justify-center">
	<h3 class="text-3xl text-center w-full my-4">FERRAMENTA DE TRABALHO</h3>
	<div class="bg-solid bg-white rounded-3xl text-center px-12 py-4 my-6 w-1/2">
		<h3 class="text-gray-400 text-3xl font-light">GPA - GALLO PERSONAL ADVANCED</h3>
	</div>
	<div class="w-full flex justify-center">
		<img src={Computer} alt="" class="computer" />
	</div>
	<div class="text-center text-3xl px-48 text-container">
		<p>
			O GPA, é a sua ferramenta para avaliar e customizar todos os programas, com total precisão,
			segurança e certeza de resultado. Software exclusivo para alunos da Certificação.
		</p>
		<p>
			Além de todo Conteúdo, todos os módulos e aulas que somam mais de 50 aulas, eu criei uma
			ferramenta fantástica que é o GPA, para processar todas informações e customizar todos os
			programas com total precisão.
		</p>
		<p>
			O software é exclusivo para alunos da Certificação e custa 600 reais a anuidade, com 10
			licenças.
		</p>
		<p>
			Obs: Cada licença representa o cadastro de 1 aluno, ou seja, com apenas uma licença você pode
			avaliar esse mesmo aluno quantas vezes você quiser, e criar quantos programas você quiser. 10
			licenças = 10 alunos
		</p>
		<p class="font-bold mb-12">Mas, pra você que vai entrar nessa turma da certificação:</p>
		<hr />
	</div>
	<div class="text-container text-center text-3xl px-96">
		<p>Ou seja, você não vai pagar anuidade por um ano, e vai ganhar mais 3 licenças.</p>
		<p>
			Após o vencimento da anuidade gratuita, o custo da anuidade é de R$ 600,00 com 10 licenças
			incluídas no pacote anual.
		</p>
		<p class="font-black">DÚVIDA: GALLO E SE EU ATENDER 10 ALUNOS NO MÊS?</p>
		<p>
			Dentro do próprio GPA, você pode comprar mais licenças por R$ 25,00 cada. O pacote com 10
			custa R$ 250,00 reais.
		</p>
	</div>
	<div class="flex justify-center flex-wrap w-full">
		<img src={SystemDemo} alt="" class="my-12 m-auto" />
	</div>
	<div class="flex justify-center flex-wrap">
		<MasterclassGradient />
	</div>
</div>

<style>
	div.card {
		background: linear-gradient(135deg, #00f583 0%, #086098 47.41%, #0083d5 100%);
	}
	img.computer {
		max-width: 1000px;
		height: auto;
	}
	div.text-container p {
		margin: 3rem 0;
	}
</style>
