<script>
    export let percentage = 0;
    const FULL_CIRCLE = 326.725; // 2 * Math.PI * 52
    $: offset = FULL_CIRCLE * (1 - (percentage / 100));
</script>

<svg>
    <circle class="bg" cx="57" cy="57" r="52" />
    <circle class="meter" cx="57" cy="57" r="52" style="stroke-dashoffset: {offset}" />
</svg>

<style>
    .bg {
        fill: none;
        stroke-width: 10px;
        stroke: #1A2C34;
    }
    .meter {
        fill: none;
        stroke-width: 10px;
        stroke-linecap: round;
        transform: rotate(-90deg);
        transform-origin: 50% 50%;
        stroke-dasharray: 326.725; 
        stroke: greenyellow;
    }
</style>
