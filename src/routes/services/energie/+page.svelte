<script>
  const features = [
    {
      title: "Installation professionnelle",
      description: "Réalisation de travaux électriques et pose de bornes de recharge conformes aux normes IRVE."
    },
    {
      title: "Maintenance & dépannage",
      description: "Interventions rapides et fiables sur les infrastructures déjà installées."
    },
    {
      title: "Équipe certifiée",
      description: "Techniciens qualifiés et certifiés pour assurer sécurité et qualité."
    },
    {
      title: "Flexibilité & réactivité",
      description: "Sous-traitance adaptée aux besoins de nos partenaires, pour un service clé en main."
    }
  ];

  import electricparking from '$lib/images/electricparkingpress.webp';
</script>

<section class="bg-gradient-to-r from-green-400 via-blue-500 to-indigo-600 text-white">
  <div class="max-w-7xl mx-auto px-6 py-24 text-center">
    <h1 class="text-4xl sm:text-5xl font-bold mb-6">ÉNERGIE</h1>
    <p class="text-lg sm:text-xl mb-8"><span class="font-bold">ECO STAF</span> Votre partenaire en sous-traitance pour l’installation de bornes électriques.</p>

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
        src={electricparking} 
        alt="Installation de borne électrique" 
        class="w-full h-auto rounded-lg shadow-lg object-cover"
      />
    </div>
  </div>
</section>



