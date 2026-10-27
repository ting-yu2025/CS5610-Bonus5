<script>
  import Counter from './lib/Counter.svelte'
  let count = $state(0)

  function updateCount(isOn){
    count += isOn ? 1 : -1
  }
</script>

<h1>My 2X2 grid</h1>
  <p>Black square: {count}</p>
  <div class="grid">
    <Counter onToggle= {updateCount} />
    <Counter onToggle= {updateCount} />
    <Counter onToggle= {updateCount} />
    <Counter onToggle= {updateCount} />
  </div>

<style>
 .grid {
   display: grid;
   grid-template-columns: 100px 100px;
   width: 200px;
   margin: 0 auto;
 }
</style>

