<script>
    // F = m * a
    let a=0,m=0;
    $: f = m*a;
</script>

<h2>Siła ruchu jednostajnie przyśpieszona</h2>
<h3>F = m * a</h3>

Masa Ciała (m) : <input type="Number" bind:value={m}/> <br/>
Przyśpieszenie ciała(a) <input type="Number" bind:value={a}/> <br/>
Siła ruchu jednostajnie przyśpieszonym (F) {f}<br/>