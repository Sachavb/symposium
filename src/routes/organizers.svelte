<script>
  export const [{ metadata: content }] = Object.values(import.meta.globEager("$content/organizers.md"))
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
          The <a target="_blank" href="https://www.researchsoft.org/">Research Software Alliance (ReSA)</a> is an international community of professionals whose
          mission is to “bring research software communities together
          to collaborate on the advancement of the research software ecosystem.” Together, they ensure that “research software and those who develop and maintain
          it are recognized and valued as fundamental and vital to research worldwide.”
        </p>
        <p class="mt-8">
          The <a target="_blank" href="https://www.esciencecenter.nl/">Netherlands eScience Center</a> is a research organization that since 2012 has been
          uniquely positioned as an independent foundation, financed by the Dutch Research Council (NWO) and the Dutch organization for IT in
          education and research (SURF). It is the national centre with the digital skills to create innovative software solutions in academic software. The core
          activities of the eScience Center are carried out by Research Software Engineers (RSEs) who are high-end, university-level specialists who do two
          things: they do research using digital technologies and methodologies, and they engineer software.
        </p>
      </div>
      <div class="w-1/3 mt-6">
        <img src={content.image1} class="my-2 w-full h-auto rounded" alt="about part 2">
      </div>
    </div>
    <br>
  </div>

  <div class="font-bold text-2xl">
    {content.title2}
  </div>
  <div>
    <ul>
      <li>
        Michelle Barker (director Research Software Alliance)
      </li>
      <li>
        Neil Chue Hong (Software Sustainability Institute, University of Edinburgh, UK)
      </li>
      <li>
       Maria Cruz (NWO Dutch Research Council)
      </li>
      <li>
        Daniel S. Katz (National Center for Supercomputing Applications (NCSA), University of Illinois, USA)
      </li>
      <li>
        Joris van Eijnatten (Netherlands eScience Center)
      </li>
    </ul>
    <br>
  </div>

   <div class="font-bold text-2xl">
    {content.title3} (Netherlands eScience Center)
  </div>
  <div>
     <ul>
        <li>Valentina Azzarà</li>
        <li>Tom Bakker</li>
        <li>Sacha van Breugel</li>
        <li>Carlos Martinez Ortiz</li>
        <li>Veronica Pang</li>
        <li>Joris van Eijnatten</li>
     </ul>
    <br>
  </div>

</div>
