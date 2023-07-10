<script lang="ts">
	import Module1 from '$lib/img/modules/module_1.png';
	import ModulePicture from './ModulePicture.svelte';

	type Module = {
		picture: string;
		content: string;
	};

	const modules: Module[] = [
		{ picture: Module1, content: 'Fisiologia do exercício aplicada ao treinamento customizado.' }
	];
</script>

{#each modules as module, i}
	<ModulePicture picture={module.picture}>
		<span slot="title">MODULO {i + 1}</span>
		<span slot="content">{module.content}</span>
	</ModulePicture>
{/each}
