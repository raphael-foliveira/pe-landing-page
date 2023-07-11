<script>
	import MentorGradient from './MentorGradient.svelte';
	import Gallo2 from '$lib/img/mentor/GALLO_2.png';
	import Logo from '$lib/img/LOGO.png';
</script>

<MentorGradient>
	<div class="w-full mt-8 mb-4">
		<h2 class="text-5xl max-w-lg text-center mx-auto">Conheça seu Mentor</h2>
	</div>
	<div class="w-full flex justify-center hr-container mb-12">
		<div class="border-solid border-t-4 w-1/6 px-auto" />
	</div>

	<div class="w-1/2">
		<h3 class="text-4xl mb-8">Prof. José Carlos Gallo</h3>
		<p class="text-2xl py-2">
			Professor de Educação Física e Personal Trainer, há mais de 35 anos, Fisioterapeuta,
			Fisiologista do Exercício, Palestrante internacional, Já ministrou mais de 3000 cursos e
			palestras em Universidades e Congressos no Brasil e na América do Sul.
		</p>
		<p class="text-2xl py-2">
			Ex-estudante de Engenharia de Minas, Jose Carlos Gallo abriu mão da faculdade de engenharia no
			6° período e resolveu seguir o seu sonho de se tornar profissional de Educação Física,
			contrariando seu próprio pai e a todos que condenavam a sua escolha, se tornou um dos
			profissionais mais reconhecido, valorizados e bem pagos do Brasil, atingindo a marca de mais
			RS 150.000,00 por mês, atuando como Personal Trainer.
		</p>
		<p class="text-2xl py-2">
			Criador do Método Customizado a sua missão é ajudar os Profissionais de Educação Física a
			conquistar o sucesso atuando como Personal Trainer.
		</p>
	</div>
	<div class="w-1/3 flex justify-center relative">
		<img src={Gallo2} alt="Foto do mentor" class="object-cover max-w-sm absolute" />
		<img
			src={Logo}
			alt=""
			class="object-cover w-60 z-20 mt-auto ml-auto absolute bottom-8 right-20"
		/>
	</div>
</MentorGradient>

<style>
	div.hr-container * {
		border-color: #444;
	}
</style>
