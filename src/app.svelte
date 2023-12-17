<script lang="ts">
    import Index from "./pages/index.svelte"
    import Error from "./pages/error.svelte"

    const currentRoute: string = document.location.pathname
</script>

{#if currentRoute === "/"}
    <Index />
{:else}
    <Error />
{/if}
