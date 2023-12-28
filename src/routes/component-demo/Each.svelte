<script lang='ts'>
    export let gornjaGranica: number;
    $: elementi = [...Array(gornjaGranica).keys()]
</script>

{#each elementi as e}
    <div>{e}</div>
{/each}