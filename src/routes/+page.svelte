<script>
	import AboutSection from '$lib/components/AboutSection.svelte';
	import ContentSection from '$lib/components/ContentSection.svelte';
	import Masterclass from '$lib/components/Masterclass.svelte';
	import Products from '$lib/components/Products.svelte';
	import TopVideoBanner from '$lib/components/TopVideoBanner.svelte';
	import GradientContainer from '$lib/components/containers/GradientContainer.svelte';
</script>

<TopVideoBanner />
<Masterclass />
<AboutSection />
<GradientContainer>
	<Products />
	<ContentSection />
</GradientContainer>
