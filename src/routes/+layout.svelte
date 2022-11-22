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

<!-- to fix, remove anything above this line or move it below the "slot" -->

<slot />
