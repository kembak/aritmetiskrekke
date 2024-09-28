<script>
    let a1 = 18
    let k = 12
    let an = 0
    let n = 0
    let sn = 0
 function rekke(n) {
    if (n>0) {
        an = a1 + (n-1)*k
    }
 }
 function sum(n) {
    rekke(n)
    sn = ((a1+an)/2)*n
 }
</script>
<div style="margin:2rem;font-family:Arial, Helvetica, sans-serif">
<h1>Aritmetisk rekke</h1>
<h3>Vi har gitt rekka 18 + 30 + 42 + 54 + ...</h3>
<span><b>n:</b></span>
<input type="number" bind:value={n} on:change={sum(n)}>
<br><br>
<p><b>A<sub>{n}</sub></b> = {an}</p>
<p><b>S<sub>{n}</sub></b> = {sn}</p>
</div>