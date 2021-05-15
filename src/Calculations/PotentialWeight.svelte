<script>
    // p = m*v
    let m=0,g=10,h=0;
    $: Ep = m*g*h;
</script>

<h2>Energia potencjalna ciężkości</h2>
<h3>p = m * v</h3>

Masa Ciała (m) : <input type="Number" bind:value={m}/> <br/>
Przyśpieszenie ziemskie (g) <input type="Number" bind:value={g}/> <br/>
Wysokość (h) <input type="Number" bind:value={h}/> <br/>
Energia potencjalna ciężkości (Ep) <span>{Ep} J</span><br/>