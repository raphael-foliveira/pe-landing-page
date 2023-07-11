<script lang="ts">
	// The ordering of these imports is critical to your app working properly
	import '../theme.postcss';
	// If you have source.organizeImports set to true in VSCode, then it will auto change this ordering
	import '@skeletonlabs/skeleton/styles/skeleton.css';
	// Most of your app wide CSS should be put in this file
	import { AppShell } from '@skeletonlabs/skeleton';
	import '../app.postcss';
	import LOGO from '../lib/img/LOGO.png';
</script>

<!-- App Shell -->
<AppShell>
	<head>
		<title>Gallo Personal Systems</title>
	</head>
	<!-- App Bar -->
	<div class="flex flex-row w-full justify-around p-2 lg:p-4 navbar font-semibold">
		<img src={LOGO} alt="Gallo logo" />
		<a href="/" class="hidden lg:inline">Além da ED. Física</a>
		<a href="/" class="hidden lg:inline">Nossos Produtos</a>
		<a href="/" class="hidden lg:inline">Missão</a>
		<a href="/" class="hidden lg:inline">Quem somos</a>
		<a href="/" class="hidden lg:inline">Youtube</a>
		<a href="/" class="hidden lg:inline">Fale Conosco</a>
	</div>
	<!-- Page Route Content -->
	<slot />
</AppShell>

<style>
	.navbar {
		background-color: #f0f0f0;
	}
	.navbar a {
		margin: auto;
	}
</style>
