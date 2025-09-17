<script>
  import { animate } from "motion";
  import { onMount } from "svelte";

  let cards;

  onMount(() => {
    // animation en cascade des cartes
    animate(
      cards.children,
      { opacity: [0, 1], y: [40, 0] },
      { duration: 0.8, delay: (i) => i * 0.2 }
    );
  });
</script>

<section id="services" class="relative py-20">
  <div class="max-w-7xl mx-auto px-6 lg:px-12 text-center">
    <h2 class="text-3xl sm:text-4xl font-bold ">
      Nos Services
    </h2>
    <p class="mt-4 text-lg  max-w-2xl mx-auto">
      Des solutions modernes et sécurisées pour répondre à vos besoins.
    </p>

    <div
      bind:this={cards}
      class="mt-12 grid gap-8 sm:grid-cols-2 lg:grid-cols-3"
    >
      <!-- Énergie -->
      <div class="p-8 rounded-2xl shadow-lg border  hover:shadow-2xl transition transform hover:-translate-y-2">
        <div class=" text-5xl mb-4">⚡</div>
        <h3 class="text-xl font-semibold ">Énergie</h3>
        <p class="mt-3 ">
          Installation et maintenance électriques fiables, adaptées à tous types de locaux.
        </p>
      </div>

      <!-- Télécom -->
      <div class="p-8 rounded-2xl shadow-lg border  hover:shadow-2xl transition transform hover:-translate-y-2">
        <div class=" text-5xl mb-4">🌐</div>
        <h3 class="text-xl font-semibold "><a href="/services/telecom">Télécom</a></h3>
        <p class="mt-3 ">
          Solutions fibre optique et réseaux télécom performants pour vos besoins professionnels.
        </p>
      </div>

      <!-- Technologie -->
      <div class="p-8 rounded-2xl shadow-lg border  hover:shadow-2xl transition transform hover:-translate-y-2">
        <div class=" text-5xl mb-4">💻</div>
        <h3 class="text-xl font-semibold ">Technologie</h3>
        <p class="mt-3 ">
          Intégration de systèmes technologiques innovants pour un avenir connecté.
        </p>
      </div>
    </div>
  </div>
</section>
