<script>
    // v = a*t
    let a=0,t=0;
    $: v = a*t;
</script>

<h2>Prędkość  w ruchu jedno-stajnie przyspieszonym</h2>
<h3>v = a * t</h3>

Przyśpieszenie (a) : <input type="Number" bind:value={a}/> <br/>
Czas (t) <input type="Number" bind:value={t}/> <br/>
Prędkość (v) {v} (m/s)<br/>