<script lang='ts'>
    let ime:string= "";
    let prezime:string ="";
</script>

<input type="text" bind:value={ime}>
<input type="text" bind:value={prezime}>

{#if ime.length === 0 && prezime.length === 0}
    <h1>Unesite vrednost za ime i za prezime</h1>
{:else}
    <h1>Zdravo ja sam {ime} {prezime}</h1>
{/if}
