<script>
	import '../global.css';
	import { navigating } from '$app/stores';
</script>

<svelte:head>
	<title>Wierd</title>
</svelte:head>

{#if $navigating}
	<span>spagetti?</span>
{/if}

<slot />
