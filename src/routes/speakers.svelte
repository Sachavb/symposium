<script>
  import SpeakersIntroduction from "$content/speakers.md";

  export const [{ metadata }] = Object.values(import.meta.globEager("$content/speakers.md"))
</script>

<div class="container mx-auto mb-16 w-full text-center">
  <div class=" mt-10 max-w-4xl mx-auto text-left ">
    <SpeakersIntroduction/>
  </div>

  <section class="container mx-auto flex flex-wrap pb-10">
    {#each metadata.members as member}
      <div class="p-4 w-full sm:w-1/2 lg:w-1/3">
        <div class="flex flex-col h-full p-4 items-center rounded shadow bg-white">
          <img width="200" height="200" class="rounded-full object-cover w-30 h-30" alt={member.name} src={member.image}>
          <div class="w-full lg:pl-6 p-4">
            <h4 class="mb-2 text-2xl font-bold font-heading">
              { member.name }
            </h4>
            <p class="mb-4 text-gray-700 leading-loose">{ member.desc }</p>
          </div>
        </div>
      </div>
    {/each}
  </section>

  <div id="secretariat" class="p-4 mb-20">
    <h2 class="text-2xl font-bold mt-10">
      Host
    </h2>
    <p class="mb-10">
      Host description
    </p>

    <div class="p-4 w-full sm:w-1/2 lg:w-1/3">
      <div class="flex flex-col h-full p-4 items-center rounded shadow bg-white">
        <img width="200" height="200" class="rounded-full object-cover w-30" alt={metadata.host.name} src={metadata.host.image}>
        <div class="w-full lg:pl-6 p-4">
          <h4 class="mb-2 text-2xl font-bold font-heading">
            { metadata.host.name }
          </h4>
          <p class="mb-4 text-gray-700 leading-loose">{ metadata.host.desc }</p>
        </div>
      </div>
    </div>
  </div>
</div>
