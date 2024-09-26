<script>
    let a1 = 18
    let k = 12
    let i = 1
    let an = 0
    let n = 0
 function rekke(n) {
    if (n>0) {
        an = a1 + (n-1)*k
    }
 }
 function sum(n) {
    while (i<=n) {
        an = a1 + (n-1)*k
        i = i+1
    }
 }
</script>
<input type="number" bind:value={n}>
<button on:click={rekke(n)}>rekke</button>
<p>{an}</p>