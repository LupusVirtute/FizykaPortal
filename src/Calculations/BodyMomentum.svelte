<script>
    // p = m*v
    let m=0,v=0;
    $: p = m*v;
</script>

<h2>Pęd ciała</h2>
<h3>p = m * v</h3>

Masa Ciała (m) : <input type="Number" bind:value={m}/> <br/>
Prędkośc (v) <input type="Number" bind:value={v}/> <br/>
Pęd (p) {p} kg * (m/s)<br/>