<script>
    import { Button, TextBlock } from "fluent-svelte";
    import "fluent-svelte/theme.css";

    let count = 0;
</script>

<div class="align-mid">
    <TextBlock variant="display">{count}.</TextBlock>
    <div>
        <Button variant="accent" on:click={() => count++}>Increase Counter</Button>
        <Button on:click={() => count = 0}>Reset Counter</Button>
    </div>
</div>
<style>
    .align-mid {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        margin: 0;
        width: 100vw;
        height: 100vh;
        background-color: #202020;
    }
    :global(body) {
		margin: 0;
		padding: 0;
        color: var(--fds-text-primary);
	}
</style>