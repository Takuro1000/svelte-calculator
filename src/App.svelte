<script lang="ts">
  //alert("welcome to svelte calculator!");
</script>

<main class="space-y-8">
  <div class="flex flex-col items-center justify-center min-h-screen bg-gray-100 text-gray-800">
    <h1 class="text-4xl font-bold mb-8">SVELTE CALCULATOR</h1>
    <div class="mb-4">
      <input class="border border-gray-300 rounded px-3 py-2 mr-2" type="text" placeholder="input number 1">
      <input class="border border-gray-300 rounded px-3 py-2" type="text" placeholder="input number 2">
    </div>
    <div class="mb-4 space-x-4">
      <button class="px-4 py-2 bg-blue-500 text-white rounded hover:bg-blue-700">ADD</button>
      <button class="px-4 py-2 bg-green-500 text-white rounded hover:bg-green-700">SUBTRACT</button>
      <button class="px-4 py-2 bg-yellow-500 text-white rounded hover:bg-yellow-700">MULTIPLY</button>
      <button class="px-4 py-2 bg-red-500 text-white rounded hover:bg-red-700">DIVIDE</button>
    </div>
    <div>
      <h2 class="text-2xl font-semibold">Result: 0</h2>
    </div>
  </div>
</main>
