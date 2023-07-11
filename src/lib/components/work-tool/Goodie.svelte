<script lang="ts">
	export let image: string;
	export let text: string;
</script>

<div class="flex flex-wrap justify-center w-1/3 my-4">
	<div class="flex flex-wrap justify-center w-full mb-4">
		<img src={image} alt="" class="h-20 w-auto" />
	</div>
	<p class="text-xl text-center max-w-xs">{text}</p>
</div>
