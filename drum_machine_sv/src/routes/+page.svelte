<script>
    const buttons = Array.from({ length: 20 }, (_, i) => i + 1);
</script>
  
<div class="w-full p-4">
  <div class="flex w-full">
    <div class="flex flex-col gap-3 justify-center items-center w-1/3">
      <label for="Quantity" class="sr-only"> Quantity </label>
      <div class="flex items-center gap-1">
        <button type="button" class="size-10 leading-10 text-gray-600 transition hover:opacity-75">
          &minus;
        </button>
        <input
          type="number"
          id="Quantity"
          value="1"
          class="h-10 w-16 rounded-sm border-gray-200 text-center [-moz-appearance:_textfield] sm:text-sm [&::-webkit-inner-spin-button]:m-0 [&::-webkit-outer-spin-button]:m-0"
        />
        <button type="button" class="size-10 leading-10 text-gray-600 transition hover:opacity-75">
          &plus;
        </button>
      </div>
      <div class="flex items-center gap-1">
        <button type="button" class="size-10 leading-10 text-gray-600 transition hover:opacity-75">
          &minus;
        </button>
        <input
          type="number"
          id="Quantity"
          value="1"
          class="h-10 w-16 rounded-sm border-gray-200 text-center [-moz-appearance:_textfield] sm:text-sm [&::-webkit-inner-spin-button]:m-0 [&::-webkit-outer-spin-button]:m-0"
        />
        <button type="button" class="size-10 leading-10 text-gray-600 transition hover:opacity-75">
          &plus;
        </button>
      </div>
      <div class="flex items-center gap-1">
        <button type="button" class="size-10 leading-10 text-gray-600 transition hover:opacity-75">
          &minus;
        </button>
        <input
          type="number"
          id="Quantity"
          value="1"
          class="h-10 w-16 rounded-sm border-gray-200 text-center [-moz-appearance:_textfield] sm:text-sm [&::-webkit-inner-spin-button]:m-0 [&::-webkit-outer-spin-button]:m-0"
        />
        <button type="button" class="size-10 leading-10 text-gray-600 transition hover:opacity-75">
          &plus;
        </button>
      </div>
    </div>
    <div class="btngrid grid grid-cols-5 gap-y-3 w-2/3">
      {#each buttons as num, i}
        <button
          class="gridbtn aspect-square w-full"
          class:ml-4={(i % 5 === 4)}
        >
          {num}
        </button>
      {/each}
    </div>
  </div>
</div>
