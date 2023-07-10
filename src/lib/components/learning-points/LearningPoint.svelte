<script lang="ts">
	export let image: string;
	export let bottomPos: string = '0';
</script>

<div class="w-1/2 flex flex-wrap p-20">
	<div class="image-background rounded-3xl h-24 w-24 drop-shadow-md mr-8">
		<img src={image} alt="" class={`drop-shadow-lg absolute bottom-${bottomPos}`} />
	</div>
	<div class="w-10/12">
		<h3 class="text-4xl">
			<slot name="title" />
		</h3>
		<p class="text-2xl">
			<slot name="content" />
		</p>
	</div>
</div>

<style>
	.image-background {
		background-color: #00f58370;
	}
</style>
