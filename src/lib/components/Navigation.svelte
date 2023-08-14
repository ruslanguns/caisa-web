<nav
	class="fixed z-10 flex content-center justify-between w-full px-4 py-6 lg:px-48 md:px-12 bg-secondary"
>
	<div class="flex items-center text-3xl font-bold font-pt-serif">Caisa</div>
	<ul class="items-center hidden font-montserrat md:flex">
		<li class="mx-3">
			<a class="growing-underline" href="howitworks"> ¿Cómo trabajamos? </a>
		</li>
		<li class="mx-3 growing-underline">
			<a href="features">Filosofía</a>
		</li>
		<li class="mx-3 growing-underline">
			<a href="pricing">Servicios</a>
		</li>
	</ul>
	<div class="hidden font-montserrat md:block">
		<button class="px-4 py-2 text-white bg-black rounded-3xl"> ¡Habla con nosotros! </button>
	</div>
	<div id="showMenu" class="md:hidden">
		<img src="assets/logos/Menu.svg" alt="Menu icon" />
	</div>
</nav>
<div
	id="mobileNav"
	class="fixed top-0 left-0 z-20 hidden w-full h-full px-4 py-6 bg-secondary animate-fade-in-down"
>
	<div id="hideMenu" class="flex justify-end">
		<img src="assets/logos/Cross.svg" alt="" class="w-16 h-16" />
	</div>
	<ul class="flex flex-col items-center mx-8 my-24 text-3xl font-montserrat">
		<li class="my-6">
			<a href="howitworks">How it works</a>
		</li>
		<li class="my-6">
			<a href="features">Features</a>
		</li>
		<li class="my-6">
			<a href="pricing">Pricing</a>
		</li>
	</ul>
</div>
