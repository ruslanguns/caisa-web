<script>
	import GorritoIcon from './GorritoIcon.svelte';

	export let title = '';
	export let content = '';
</script>

<div class="flex items-start my-6 mr-10 font-montserrat">
	<GorritoIcon />

	<div>
		<h3 class="text-2xl font-semibold">{title}</h3>
		<p>{content}</p>
	</div>
</div>
