<script>
	import Feature from '$lib/components/Feature.svelte';
	import Navigation from '$lib/components/Navigation.svelte';
	import SegmentTitle from '$lib/components/SegmentTitle.svelte';
	import { FEATURES } from '$lib/content/features';
</script>

<!-- Navigation -->
<Navigation />

<!-- Hero -->
<section
	class="flex flex-col justify-center px-4 pt-24 text-center md:mt-0 md:h-screen md:text-left md:flex-row md:justify-between md:items-center lg:px-48 md:px-12 bg-secondary"
>
	<div class="md:flex-1 md:mr-10">
		<h1 class="text-5xl font-bold font-pt-serif mb-7">
			Reinventando
			<span class="bg-underline1 bg-left-bottom bg-no-repeat pb-2 bg-100%"> el Futuro </span>
			de Centroamérica
		</h1>
		<p class="font-normal font-pt-serif mb-7">
			Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum harum tempore consectetur
			voluptas, cumque nobis laboriosam voluptatem.
		</p>
		<div class="font-montserrat">
			<button
				class="px-6 py-4 mb-2 mr-2 text-white bg-black border-2 border-black border-solid rounded-lg"
			>
				Contactarnos
			</button>
			<button class="px-6 py-4 border-2 border-black border-solid rounded-lg"> Action </button>
		</div>
	</div>
	<div class="flex justify-around mt-8 md:block md:mt-0 md:flex-1">
		<div class="relative">
			<img src="assets/Highlight1.svg" alt="" class="absolute -top-16 -left-10" />
		</div>
		<img src="assets/project-figure.svg" alt="Macbook" />
		<div class="relative">
			<img src="assets/Highlight2.svg" alt="" class="absolute -bottom-10 -right-6" />
		</div>
	</div>
</section>

<!-- How it works . -->
<section class="text-white bg-black sectionSize">
	<SegmentTitle dark title="¿Cómo trabajamos?" />
	<div class="flex flex-col md:flex-row">
		<div class="flex flex-col items-center flex-1 mx-8 my-4">
			<div
				class="flex items-center justify-center w-12 h-12 mb-3 text-black border-2 rounded-full bg-secondary"
			>
				1
			</div>
			<h3 class="mb-2 text-xl font-medium font-montserrat">Eat</h3>
			<p class="text-center font-montserrat">
				Lorem ipsum dolor, sit amet consectetur adipisicing elit.
			</p>
		</div>
		<div class="flex flex-col items-center flex-1 mx-8 my-4">
			<div
				class="flex items-center justify-center w-12 h-12 mb-3 text-black border-2 rounded-full bg-secondary"
			>
				2
			</div>
			<h3 class="mb-2 text-xl font-medium font-montserrat">Sleep</h3>
			<p class="text-center font-montserrat">
				Lorem ipsum dolor, sit amet consectetur adipisicing elit.
			</p>
		</div>
		<div class="flex flex-col items-center flex-1 mx-8 my-4">
			<div
				class="flex items-center justify-center w-12 h-12 mb-3 text-black border-2 rounded-full bg-secondary"
			>
				3
			</div>
			<h3 class="mb-2 text-xl font-medium font-montserrat">Rave</h3>
			<p class="text-center font-montserrat">
				Lorem ipsum dolor, sit amet consectetur adipisicing elit.
			</p>
		</div>
	</div>
</section>

<!-- Features -->
<section class="sectionSize bg-secondary">
	<SegmentTitle title="Feature" />

	<div class="md:grid md:grid-cols-2 md:grid-rows-2">
		{#each FEATURES as { title, content }}
			<Feature {title} {content} />
		{/each}
	</div>
</section>

<!-- Pricing -->
<section class="py-0 sectionSize bg-secondary">
	<SegmentTitle title="Pricing" />
	<div class="flex flex-col w-full md:flex-row">
		<div
			class="relative flex flex-col flex-1 px-8 py-5 mx-6 my-8 shadow-2xl bg-secondary rounded-2xl md:top-24"
		>
			<h3 class="mb-4 text-2xl font-normal font-pt-serif">The Good</h3>
			<div class="mb-4 text-2xl font-bold font-montserrat">
				$25
				<span class="text-base font-normal"> / month</span>
			</div>

			<div class="flex">
				<img src="assets/logos/CheckedBox.svg" alt="" class="mr-1" />
				<p>Benefit #1</p>
			</div>
			<div class="flex">
				<img src="assets/logos/CheckedBox.svg" alt="" class="mr-1" />
				<p>Benefit #2</p>
			</div>
			<div class="flex">
				<img src="assets/logos/CheckedBox.svg" alt="" class="mr-1" />
				<p>Benefit #3</p>
			</div>

			<button class="py-3 mt-4 text-lg border-2 border-black border-solid rounded-xl">
				Choose plan
			</button>
		</div>

		<div
			class="relative flex flex-col flex-1 px-8 py-5 mx-6 my-8 shadow-2xl bg-secondary rounded-2xl md:top-12"
		>
			<h3 class="mb-4 text-2xl font-normal font-pt-serif">The Bad</h3>
			<div class="mb-4 text-2xl font-bold font-montserrat">
				$40
				<span class="text-base font-normal"> / month</span>
			</div>

			<div class="flex">
				<img src="assets/logos/CheckedBox.svg" alt="" class="mr-1" />
				<p>Benefit #1</p>
			</div>
			<div class="flex">
				<img src="assets/logos/CheckedBox.svg" alt="" class="mr-1" />
				<p>Benefit #2</p>
			</div>
			<div class="flex">
				<img src="assets/logos/CheckedBox.svg" alt="" class="mr-1" />
				<p>Benefit #3</p>
			</div>

			<button class="py-3 mt-4 text-lg border-2 border-black border-solid rounded-xl">
				Choose plan
			</button>
		</div>

		<div
			class="relative flex flex-col flex-1 px-8 py-5 mx-6 my-8 shadow-2xl bg-secondary rounded-2xl md:top-24"
		>
			<h3 class="mb-4 text-2xl font-normal font-pt-serif">The Ugly</h3>
			<div class="mb-4 text-2xl font-bold font-montserrat">
				$50
				<span class="text-base font-normal"> / month</span>
			</div>

			<div class="flex">
				<img src="assets/logos/CheckedBox.svg" alt="" class="mr-1" />
				<p>Benefit #1</p>
			</div>
			<div class="flex">
				<img src="assets/logos/CheckedBox.svg" alt="" class="mr-1" />
				<p>Benefit #2</p>
			</div>
			<div class="flex">
				<img src="assets/logos/CheckedBox.svg" alt="" class="mr-1" />
				<p>Benefit #3</p>
			</div>

			<button class="py-3 mt-4 text-lg border-2 border-black border-solid rounded-xl">
				Choose plan
			</button>
		</div>
	</div>
</section>

<!-- FAQ  -->
<section class="items-start pt-8 text-white bg-black sectionSize md:pt-36">
	<div>
		<h2 class="secondaryTitle bg-highlight3 p-10 mb-0 bg-center bg-100%">FAQ</h2>
	</div>

	<div class="w-full py-4">
		<div class="flex items-center justify-between">
			<div class="mr-auto font-medium font-montserrat">Where can I get this HTML template?</div>
			<img src="assets/logos/CaretRight.svg" alt="" class="transition-transform transform" />
		</div>
		<div class="hidden pb-8 text-sm font-montserrat font-extralight">
			You can download it on Gumroad.com
		</div>
	</div>
	<hr class="w-full bg-white" />

	<div class="w-full py-4">
		<div class="flex items-center justify-between">
			<div class="mr-auto font-medium font-montserrat">Is this HTML template free?</div>
			<img src="assets/logos/CaretRight.svg" alt="" class="transition-transform transform" />
		</div>
		<div class="hidden pb-8 text-sm font-montserrat font-extralight">Yes! For you it is free.</div>
	</div>
	<hr class="w-full bg-white" />

	<div class="w-full py-4">
		<div class="flex items-center justify-between">
			<div class="mr-auto font-medium font-montserrat">Am I awesome?</div>
			<img src="assets/logos/CaretRight.svg" alt="" class="transition-transform transform" />
		</div>
		<div class="hidden pb-8 text-sm font-montserrat font-extralight">Yes! No doubt about it.</div>
	</div>
	<hr class="w-full bg-white" />
</section>

<!-- Footer -->
<section class="bg-black sectionSize">
	<div class="mb-4">
		<img src="assets/Logo_white.svg" alt="Logo" class="h-4" />
	</div>
	<div class="flex mb-8">
		<a href="/">
			<img src="assets/logos/Facebook.svg" alt="Facebook logo" class="mx-4" />
		</a>
		<a href="/">
			<img src="assets/logos/Youtube.svg" alt="Youtube logo" class="mx-4" />
		</a>
		<a href="/">
			<img src="assets/logos/Instagram.svg" alt="Instagram logo" class="mx-4" />
		</a>
		<a href="/">
			<img src="assets/logos/Twitter.svg" alt="Twitter logo" class="mx-4" />
		</a>
	</div>
	<div class="text-sm text-white font-montserrat">© 2021 STARTUP. All rights reserved</div>
</section>
