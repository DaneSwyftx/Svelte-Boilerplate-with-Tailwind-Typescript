<script lang="ts">
  var counter = 0;

  function increment() {
    counter++;
  }
  
  function decrement() {
    counter--;
  }
</script>

<div class="flex text-lg mt-8 gap-4 justify-center items-center">
  <button class="bg-blue-400 p-4 text-white font-bold rounded-full" on:click={decrement}>-</button>
  <h1>{counter}</h1>
  <button class="bg-blue-400 p-4 text-white font-bold rounded-full" on:click={increment}>+</button>
</div>