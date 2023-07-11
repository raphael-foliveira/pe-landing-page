<script lang="ts">
	import LearningPoint from './LearningPoint.svelte';
	import IconArrowUp from '$lib/img/icons/icon_arrow_up_.png';
	import IconStar from '$lib/img/icons/icon_star_.png';
	import IconSearchJob from '$lib/img/icons/icon_search_job_.png';
	import IconTool from '$lib/img/icons/icon_tool_.png';
	import IconYoutube from '$lib/img/icons/icon_youtube_.png';
	import IconCoins from '$lib/img/icons/icon_coins_.png';
	import MasterclassGradient from '../masterclass/MasterclassGradient.svelte';
</script>

<div class="flex flex-wrap">
	<LearningPoint image={IconStar}>
		<span slot="title">Autoridade</span>
		<span slot="content"
			>Autoridade profissional na integração com todos o profissionais da área de saúde, DE IGUAL
			PARA IGUAL habilitado a promover diversos tratamentos de saúde através do exercício físico.</span
		>
	</LearningPoint>
	<LearningPoint image={IconSearchJob}>
		<span slot="title">Metodologia de trabalho</span>
		<span slot="content"
			>O passo a passo para você atuar com precisão, segurança e 100% DE CERTEZA de resultado em
			todas as suas prescrições e programas de treinamento.</span
		>
	</LearningPoint>
	<LearningPoint image={IconArrowUp} bottomPos="12">
		<span slot="title">Valor</span>
		<span slot="content"
			>Um portfólio que te permite faturar de R$ 3.000 A R$ 5.000 por programas de tratamento de
			saúde de acordo ao objetivo do seu aluno.</span
		>
	</LearningPoint>
	<LearningPoint image={IconTool}>
		<span slot="title">Ferramenta de trabalho exclusiva</span>
		<span slot="content"
			>Software exclusivo para alunos, para você avaliar, prescrever, priorizar e controlar todos os
			programas de treinamento customizado dos seus alunos.</span
		>
	</LearningPoint>
	<LearningPoint image={IconYoutube}>
		<span slot="title">Posicionamento, Marketing e Vendas</span>
		<span slot="content"
			>Curso completo + Mentorias ao vivo no zoom para você aprender a se posicionar da forma
			correta, se diferenciar completamente dos outros Personal que vende hora aula e vender
			programas que variam de 3 a 5 mil reais + Passo a passo de como ofertar seu serviço com alto
			valor agregado + script de fechamento de vendas..</span
		>
	</LearningPoint>
	<LearningPoint image={IconCoins}>
		<span slot="title">Metodologia de vendas</span>
		<span slot="content">
			O ambiente ideal para tirar qualquer dúvida e interagir com mais de 800 Profissionais
			certificados em todos os estados do Brasil.
		</span>
	</LearningPoint>
</div>
