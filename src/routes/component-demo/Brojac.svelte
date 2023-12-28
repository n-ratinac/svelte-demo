<script>
    let vrednost = 0;

    const inc = () => {
        vrednost++;
        console.log(vrednost);
    }

    const dec = () => {
        vrednost--;
        console.log(vrednost);
    }

    const double = () => {
        vrednost *= 2;
        console.log(vrednost);
    }
    $: pola = vrednost;
</script>

<h3>{vrednost}</h3>
<h4>Pola od {vrednost} je {pola}</h4>
<button on:click={inc}>+</button>
<button on:click={dec}>-</button>
<button on:click={double}>x2</button>