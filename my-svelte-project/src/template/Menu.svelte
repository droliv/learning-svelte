<script>
    export let logged = false;
    function toggle() {
		logged = !logged;
	}
</script>

{#if logged}
	<button on:click={toggle}>
		Log out
	</button>
{:else}
	<button on:click={toggle}>
		Log in
	</button>
{/if}