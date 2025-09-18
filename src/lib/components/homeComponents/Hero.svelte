<script>
  import { animate } from "motion";
  import { onMount } from "svelte";
  import electricimg from '$lib/images/electricpress.webp';

  let title, subtitle, buttons;

  onMount(() => {
    animate(title, { opacity: [0, 1], y: [40, 0] }, { duration: 0.8 });
    animate(subtitle, { opacity: [0, 1], y: [40, 0] }, { duration: 0.8, delay: 0.3 });
    animate(buttons, { opacity: [0, 1], y: [40, 0] }, { duration: 0.8, delay: 0.6 });
  });
</script>

<section class="relative bg-gray-900 text-white overflow-hidden">
  <!-- Background overlay -->
  <div class="absolute inset-0">
    <img 
      src={electricimg} 
      alt="Électricité et fibre optique" 
      class="w-full h-full object-cover opacity-30" 
    />
    <div class="absolute inset-0 bg-black/60"></div>
  </div>

  <div class="relative z-10 max-w-7xl mx-auto px-6 lg:px-12 py-32 text-center">
    <h1
      bind:this={title}
      class="text-4xl sm:text-6xl font-extrabold leading-tight opacity-0"
    >
      Travaux d'installation électrique <br />
      <span class="text-blue-400">& fibre optique</span> dans tous locaux
    </h1>

    <p
      bind:this={subtitle}
      class="mt-6 text-lg sm:text-xl text-gray-300 max-w-2xl mx-auto opacity-0"
    >
      Des solutions modernes, sécurisées et adaptées à vos besoins professionnels et résidentiels.
    </p>

    <div
      bind:this={buttons}
      class="mt-8 flex justify-center gap-4 opacity-0"
    >
      <a
        href="/contactUS"
        class="px-6 py-3 rounded-2xl bg-blue-500 hover:bg-blue-600 transition shadow-lg font-semibold"
      >
        Contactez-nous
      </a>

    </div>
  </div>

  <!-- Decorative bottom wave -->
  <div class="absolute bottom-0 left-0 right-0">
    <svg
      class="w-full h-20 text-base-100"
      preserveAspectRatio="none"
      viewBox="0 0 1440 320"
      fill="currentColor"
    >
      <path
        fill="currentColor"
        d="M0,96L80,106.7C160,117,320,139,480,149.3C640,160,800,160,960,133.3C1120,107,1280,53,1360,26.7L1440,0L1440,320L1360,320C1280,320,1120,320,960,320C800,320,640,320,480,320C320,320,160,320,80,320L0,320Z"
      ></path>
    </svg>
  </div>
</section>
