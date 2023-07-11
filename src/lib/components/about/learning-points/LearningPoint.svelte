<script lang="ts">
	export let image: string;
	export let bottomPos: string = '0';
</script>

<div
	class="w-full lg:w-1/2 flex flex-wrap justify-center text-center px-8 lg:justify-normal lg:text-left lg:px-0 py-4 lg:py-20"
>
	<div
		class="image-background rounded-3xl h-24 w-24 drop-shadow-md lg:mr-8 mb-8 flex justify-center"
	>
		<img src={image} alt="" class="object-contain drop-shadow-lg absolute bottom-{bottomPos}" />
	</div>
	<div class="lg:w-2/3">
		<h3 class="lg:text-4xl text-2xl font-bold">
			<slot name="title" />
		</h3>
		<p class="lg:text-2xl text-xl">
			<slot name="content" />
		</p>
	</div>
</div>

<style>
	.image-background {
		background-color: #00f58370;
	}
</style>
