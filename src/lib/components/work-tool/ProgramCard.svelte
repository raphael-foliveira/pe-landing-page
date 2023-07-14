<script lang="ts">
	export let title: string;
	export let image: string;
</script>

<div class="rounded-3xl p-4 lg:p-8 flex flex-wrap card-wrapper my-12 justify-between">
	<div class="w-full lg:w-3/5 py-4">
		<h3 class="text-4xl">
			{title.toUpperCase()}
		</h3>
		<div class="text-xl">
			<slot />
		</div>
	</div>
	<div class="w-full lg:w-2/5 py-8 flex justify-center">
		<img src={image} alt="" class="object-contain w-full" />
	</div>
</div>

<style>
	div.card-wrapper {
		background-color: #f8f8f8;
	}

	h3 {
		background: linear-gradient(0deg, #003252 0%, #0097f5 100%);
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
		background-clip: text;
		color: transparent;
	}
</style>
