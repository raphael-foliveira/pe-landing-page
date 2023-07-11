<script>
	import InvestmentCard from './InvestmentCard.svelte';
	import InvestmentGradient from './InvestmentGradient.svelte';
</script>

<InvestmentGradient>
	<h3 class="text-center text-5xl my-8 w-full">VALOR DO INVESTIMENTO</h3>
	<InvestmentCard />
	<button class="py-4 px-12 text-3xl font-black rounded-3xl w-2/3 my-32 mb-12"
		>QUERO ME INSCREVER</button
	>
</InvestmentGradient>

<style>
	h3 {
		color: #00f583;
	}
	button {
		background-color: #00f583;
		color: #003252;
	}
</style>
