<script>
    import stafImg from '$lib/images/staf.webp';
</script>

<section class="ezy__about9 light py-14 md:py-24 hero">
  <div class="container px-4">
    <div class="grid grid-cols-12 items-center gap-4 mb-12">
      <div class="col-span-12 lg:col-span-6">
        
        <h1 class="text-3xl leading-none font-bold uppercase tracking-wider mb-2  text-blue-900">Bienvenue à ECO STAF</h1>
        <hr class="bg-blue-600 h-1 rounded-[3px] w-12 opacity-100 my-6" />
        <p class=" mb-2">
          Spécialisée dans les travaux d’installation électrique et fibre optique dans tous locaux,
nous proposons des solutions modernes, sécurisées et adaptées à vos besoins professionnels comme résidentiels.
        </p>
        <ul class="flex flex-col ezy__about9-features mt-5 font-semibold">
          <li>
            <span class="fas fa-check text-blue-600 mr-2 mb-4 text-sm"></span>
            <span class=" text-sm ">Solutions modernes</span>
          </li>
          <hr class="w-11/12 my-2" />
          <li>
            <span class="fas fa-check text-blue-600 mr-2 mb-4 text-sm"></span>
            <span class=" text-sm">Sécurité renforcée</span>
          </li>
          <hr class="w-11/12 my-2" />
          <li>
            <span class="fas fa-check text-blue-600 mr-2 mb-4 text-sm"></span>
            <span class=" text-sm">Adaptées à vos besoins</span>
          </li>
          <hr class="w-11/12 my-2" />
          <li>
            <span class="fas fa-check text-blue-600 mr-2 mb-4 text-sm"></span>
            <span class=" text-sm">Accompagnement professionnel</span>
          </li>
          <hr class="w-11/12 my-2" />
          <li>
            <span class="fas fa-check text-blue-600 mr-2 text-sm"></span>
            <span class="text-sm">Fiabilité garantie</span>
          </li>
        </ul>
        <div class="mt-12">
          <a href="/about"
            class="bg-blue-500 text-white font-semibold btn rounded-md px-5 py-2 transition"
          >
            En savoir plus
        </a>
        </div>
      </div>
      <div class="col-span-12 lg:col-span-6">
        <div class="mt-12 lg:mt-0">
          <img
            src={stafImg}
            alt=""
            class="max-w-full h-auto rounded-2xl"
          />
        </div>
      </div>
    </div>
  </div>
</section>
