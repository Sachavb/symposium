<script>
  export const [{ metadata: content }] = Object.values(import.meta.globEager("$content/accommodation.md"))
</script>

<svelte:head>
  <title>About</title>
</svelte:head>

<div class="max-w-screen-lg w-full mx-auto pt-20 px-3">
  <div class="font-bold text-2xl">
    {content.title1}
  </div>

  <div>
    <div class="flex gap-4">
      <div class="w-2/3">
        <p class="">
          More information coming soon...
        </p>
        <p class="mt-8">
          
        </p>
      </div>
      <div class="w-1/3 mt-6">
        <img src={content.image1} class="my-2 w-full h-auto rounded" alt="about part 2">
      </div>
    </div>
    <br>
  </div>
</div>
