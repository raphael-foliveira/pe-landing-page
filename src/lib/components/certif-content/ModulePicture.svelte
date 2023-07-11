<script lang="ts">
	export let picture: string;
</script>

<div class="w-full lg:w-1/3 my-8 lg:px-12 flex justify-center">
	<div class="module-background bg-cover w-full" style={`background-image: url(${picture})`}>
		<div class="module-container py-12 flex flex-wrap justify-center h-full text-center text-white">
			<div class="w-full lg:mx-32 mb-8 px-20">
				<h3 class="text-2xl lg:text-4xl p-2">
					<slot name="title" />
				</h3>
			</div>
			<div>
				<p class="text-xl lg:text-3xl lg:px-8 px-6">
					<slot name="content" />
				</p>
			</div>
		</div>
	</div>
</div>

<style>
	.module-background {
		/* height: 635px;
		width: 490px; */
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
