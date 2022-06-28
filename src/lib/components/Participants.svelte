<script>
  export const [{ metadata: { participants } }] = Object.values(import.meta.globEager("$content/participants.md"))
</script>

<div id="participants" class="bg-white p-10 flex flex-wrap gap-10 container mx-auto my-20">
  <h2 class="text-2xl font-medium mb-10">Confirmed participants</h2>
  <div class="flex flex-wrap gap-10 container mx-auto">
    {#each participants as item}
      <a class="mt-6 hover:opacity-80" target="_blank" href={item.link}>
        <img class="max-h-[60px]" src="{item.image}" alt="{item.image}"/>
      </a>
    {/each}
  </div>
</div>









