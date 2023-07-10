<script>
	import Rectangle1 from '$lib/img/products/Rectangle_52.png';
	import Rectangle2 from '$lib/img/products/Rectangle_53.png';
	import Rectangle3 from '$lib/img/products/Rectangle_54.png';
	import Rectangle4 from '$lib/img/products/Rectangle_55.png';
	import Rectangle5 from '$lib/img/products/Rectangle_56.png';
	import Rectangle6 from '$lib/img/products/Rectangle_57.png';
	import Rectangle7 from '$lib/img/products/Rectangle_58.png';
	import Rectangle8 from '$lib/img/products/Rectangle_59.png';
	import Rectangle9 from '$lib/img/products/Rectangle_60.png';

	const pictures = [
		Rectangle2,
		Rectangle1,
		Rectangle3,
		Rectangle4,
		Rectangle5,
		Rectangle6,
		Rectangle7,
		Rectangle8,
		Rectangle9
	];
</script>

{#each pictures as pic}
	<div class="p-8">
		<img src={pic} alt="" class="h-60 w-auto" />
	</div>
{/each}
