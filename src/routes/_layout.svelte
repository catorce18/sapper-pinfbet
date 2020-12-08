<script>
	import Nav from '../components/Nav.svelte';
	import Apuesta from '../components/Apuesta.svelte';
	export let segment;
</script>

{#if (segment !== undefined && segment !== 'index')}
<Nav {segment}/>
{/if}

{#if (segment == 'about')}
<Apuesta {segment}/>
{/if}

<main>
	<slot></slot>
</main>
