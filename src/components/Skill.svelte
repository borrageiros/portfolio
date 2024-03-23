<script>
    export let title = "";
    export let link = "";
    export let img = "";
    export let svg = "";
    const isSvg = () => svg !== "";
</script>

<style>
    .card {
        border: 5px solid transparent;
        padding: 10px;
        transition: border-color 0.3s ease;
        max-width: 30vh;
        min-width: 30vh;
        max-height: 30vh;
        min-height: 30vh;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        text-align: center;
    }
    .card:hover {
        border-color: yellowgreen;
    }
    .card img, .card .svg {
        max-width: 20vh;
        min-width: 20vh;
        max-height: 20vh;
        min-height: 20vh;
        overflow: hidden;
    }
    .card .svg {
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .card a{
        text-decoration: none;
        color: inherit;
        overflow: hidden;

        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }
    .card a p {
        margin-bottom: 10px;
    }
</style>

<div class="card">
    <a href="{link}" target="_blank">
        <p>{title}</p>
        {#if isSvg()}
            <div class='svg'>{@html svg}</div>
        {:else}
            <img src="{img}" alt="{title}" />
        {/if}
    </a>
</div>