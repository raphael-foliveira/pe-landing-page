<script lang="ts">
	import Module1 from '$lib/img/modules/module_1.png';
	import Module2 from '$lib/img/modules/module_2.png';
	import Module3 from '$lib/img/modules/module_3.png';
	import Module4 from '$lib/img/modules/module_4.png';
	import Module5 from '$lib/img/modules/module_5.png';
	import Module6 from '$lib/img/modules/module_6.png';
	import Module7 from '$lib/img/modules/module_7.png';
	import ExtraModule from '$lib/img/modules/extra_module.png';
	import ModulePicture from './ModulePicture.svelte';

	type Module = {
		picture: string;
		content: string;
	};

	const modules: Module[] = [
		{ picture: Module1, content: 'Fisiologia do exercício aplicada ao treinamento customizado.' },
		{ picture: Module2, content: 'Avaliação da aptidão física, saúde e padrões de normalidade.' },
		{
			picture: Module3,
			content:
				'Prescrição e periodização do Treinamento Aeróbico para iniciantes, intermediário e avançado para diversos objetivos.'
		},
		{
			picture: Module4,
			content:
				'Prescrição e periodização do Treinamento de Força para iniciantes, intermediário e avançado para diversos objetivos.'
		},
		{
			picture: Module5,
			content: 'Nutrição Recursos ergogênicos para hipertrofia, emagrecimento e saúde.'
		},
		{
			picture: Module6,
			content:
				'Biomecânica aplicada ao exercício e Anatomia palpatória e treinamento de realinhamento patelar e fortalecimento do joelho e coluna.'
		},
		{
			picture: Module7,
			content:
				'Aqui você aprende toda base, para prescrever programas para os grupos especiais: (Obeso, hipertenso, diabético, idoso, revascularização na fase lll da reabilitação cardíaca) e mulheres de acordo ao ciclo menstrual.'
		},
		{
			picture: ExtraModule,
			content:
				'Nesse módulo, conta com diversos tipos de programas, para facilita a sua escolha do programa, de acordo a cada tipo de cliente e objetivo e como conduzir os programas.'
		}
	];
</script>

{#each modules as module, i}
	<ModulePicture picture={module.picture}>
		<span slot="title">MODULO {i + 1}</span>
		<span slot="content">{module.content}</span>
	</ModulePicture>
{/each}
