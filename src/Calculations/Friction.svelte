<script>
    // T = f * Fn
    let f=0,fN=0;
    $: T = f*fN;
</script>

<h2>Siła tarcia</h2>
<h3> T = f * Fn </h3>

Współczynnik tarcia (f) : <input type="Number" bind:value={f}/> <br/>
Siła nacisku (Fn) <input type="Number" bind:value={fN}/> <br/>
Siła tarcia (T) <span>{T}N</span><br/>