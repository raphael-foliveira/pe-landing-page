<script>
	import MasterclassSection from '$lib/components/masterclass/MasterclassSection.svelte';
	import AboutSection from '$lib/components/about/AboutSection.svelte';
	import ContentSection from '$lib/components/certif-content/ContentSection.svelte';
	import GradientContainer from '$lib/components/containers/GradientContainer.svelte';
	import InvestmentSection from '$lib/components/investment/InvestmentSection.svelte';
	import ProductsSection from '$lib/components/products/ProductsSection.svelte';
	import TopVideoBanner from '$lib/components/video-banner/TopVideoBanner.svelte';
	import WorkToolSection from '$lib/components/work-tool/WorkToolSection.svelte';
	import MentorSection from '$lib/components/mentor/MentorSection.svelte';
</script>

<TopVideoBanner />
<MasterclassSection />
<AboutSection />
<GradientContainer>
	<ProductsSection />
	<ContentSection />
</GradientContainer>
<WorkToolSection />
<InvestmentSection />
<MentorSection />
