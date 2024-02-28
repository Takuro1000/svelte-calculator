<script lang="ts">
  let result = 0;
  let num1 = "0";  
  let num2 = "0";

  const add = () => {
    try {
      result = parseInt(num1) + parseInt(num2);
    } catch (error) {
      console.log(error);
    }
  }
  const subtract = () => {
    try {
      result = parseInt(num1) - parseInt(num2);
    } catch (error) {
      console.log(error);
    }
  }
  const multiply = () => {
    try {
      result = parseInt(num1) * parseInt(num2);
    } catch (error) {
      console.log(error);
    }
  }
  const divide = () => {
    try {
      result = parseInt(num1) / parseInt(num2);
    } catch (error) {
      console.log(error);
    }
  }
</script>

<main class="space-y-8">
  <div class="flex flex-col items-center justify-center min-h-screen bg-gray-100 text-gray-800">
    <h1 class="text-4xl font-bold mb-8">SVELTE CALCULATOR</h1>
    <div class="mb-4">
      <input class="border border-gray-300 rounded px-3 py-2 mr-2" type="text" placeholder="input number 1" bind:value={num1}>
      <input class="border border-gray-300 rounded px-3 py-2" type="text" placeholder="input number 2" bind:value={num2}>
    </div>
    <div class="mb-4 space-x-4">
      <button class="px-4 py-2 bg-blue-500 text-white rounded hover:bg-blue-700" on:click={add}>ADD</button>
      <button class="px-4 py-2 bg-green-500 text-white rounded hover:bg-green-700" on:click={subtract}>SUBTRACT</button>
      <button class="px-4 py-2 bg-yellow-500 text-white rounded hover:bg-yellow-700" on:click={multiply}>MULTIPLY</button>
      <button class="px-4 py-2 bg-red-500 text-white rounded hover:bg-red-700" on:click={divide}>DIVIDE</button>
    </div>
    <div>
      <h2 class="text-2xl font-semibold">Result : {result}</h2>
    </div>
  </div>
</main>
