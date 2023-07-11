<script lang="ts">
	export let toggleVideoFunction: () => void;
</script>

<div
	class="absolute top-0 left-0 w-full h-screen z-50 backdrop-wrapper flex justify-center"
	on:click={toggleVideoFunction}
	on:keypress
>
	<iframe
		class="my-auto"
		width="1120"
		height="630"
		src="https://www.youtube.com/embed/LpnMhSIEqfA?controls=0"
		title="YouTube video player"
		frameborder="0"
		allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
		allowfullscreen
	/>
</div>

<style>
	.backdrop-wrapper {
		backdrop-filter: brightness(0.2);
	}
</style>
