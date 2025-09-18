<script>
  const features = [
    {
      title: "Installation complète",
      description: "Études, tirage, soudure et raccordement de câbles fibre optique conformes aux normes."
    },
    {
      title: "Tous types de locaux",
      description: "Interventions dans les immeubles, bureaux, commerces, sites industriels et bâtiments publics."
    },
    {
      title: "Techniciens qualifiés",
      description: "Experts en réseaux FTTH / FTTB / FTTO avec certifications reconnues."
    },
    {
      title: "Maintenance & dépannage",
      description: "Assistance rapide et fiable pour garantir la continuité de vos services."
    }
  ];

  import opticalfiberimg from '$lib/images/opticalfiber.webp';
</script>

<section class="bg-gradient-to-r from-green-400 via-blue-500 to-indigo-600 text-white">
  <div class="max-w-7xl mx-auto px-6 py-24 text-center">
    <h1 class="text-4xl sm:text-5xl font-bold mb-6">TÉLÉCOM</h1>
    <p class="text-lg sm:text-xl"><span class="font-bold">ECO STAF</span> Des solutions fibre optique rapides, sûres et durables pour tous vos espaces.</p>

  </div>
</section>

<section id="services" class="py-20 ">
  <div class="max-w-7xl mx-auto px-6">
    
    <div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-8">
      {#each features as feature}
        <div class=" p-6 rounded-lg shadow hover:shadow-lg transition">
          <h3 class="text-xl font-semibold mb-2">{feature.title}</h3>
          <p class="">{feature.description}</p>
        </div>
      {/each}
    </div>
  </div>
</section>



<!-- Image Section -->
<section class="py-16 ">
  <div class="max-w-7xl mx-auto px-6 flex justify-center">
    <div class="w-full sm:w-3/4 lg:w-1/2">
      <img 
        src={opticalfiberimg} 
        alt="Installation de borne électrique" 
        class="w-full h-auto rounded-lg shadow-lg object-cover"
      />
    </div>
  </div>
</section>



