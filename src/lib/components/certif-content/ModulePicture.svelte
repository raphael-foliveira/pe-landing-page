<script lang="ts">
	export let picture: string;
</script>

<div
	class="bg-cover module-background h-48 w-auto my-8"
	style={`background-image: url(${picture})`}
>
	<div class="module-container flex flex-wrap justify-center text-center h-full text-white">
		<div class="w-full mx-32 mt-auto mb-8">
			<h3 class="text-4xl p-2">
				<slot name="title" />
			</h3>
		</div>
		<div>
			<p class="text-3xl px-8">
				<slot name="content" />
			</p>
		</div>
	</div>
</div>

<style>
	.module-background {
		height: 635px;
		width: 490px;
		border-radius: 51px;
	}

	h3 {
		border-bottom: solid 5px white;
	}

	.module-container {
		border-radius: 51px;
		background-color: rgba(0, 0, 0, 0.7);
	}
</style>
