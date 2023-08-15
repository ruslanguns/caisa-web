<script>
	export let dark = false;
	export let title = '';
</script>

<div>
	<h2 class:bg-underline2={dark} class:bg-underline3={!dark} class="secondaryTitle bg-100%">
		{title}
	</h2>
</div>
