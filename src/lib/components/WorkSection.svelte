<script lang="ts">
  const projects = [
    {
      client: "Fresh Produce Distribution",
      desc: "Daily delivery of premium fruits and vegetables to Bahrain's top hotels and restaurants.",
      bg: "bg-[#1a1a1a]",
      img: "/generated/image-modern-temperature-controlled-warehouse--1765530561506-0.webp",
      dark: true
    },
    {
      client: "Protein & Seafood Supply",
      desc: "Premium meat, poultry, and fresh seafood sourced from trusted global suppliers.",
      bg: "bg-gray-200",
      img: "/generated/image-premium-fresh-seafood-and-meat-displayed-1765530564465-1.webp",
      dark: false
    },
    {
      client: "Dairy & Bakery Products",
      desc: "Fresh dairy products and artisan bakery items delivered daily.",
      bg: "bg-[#f5f5f5]",
      img: "/generated/image-fresh-dairy-products-and-artisan-bread-d-1765530567607-2.webp",
      dark: false
    },
    {
      client: "Cold Chain Logistics",
      desc: "Temperature-controlled distribution ensuring freshness from source to kitchen.",
      bg: "bg-black",
      img: "/generated/image-refrigerated-delivery-truck-with-tempera-1765530569926-3.webp",
      dark: true
    },
    {
      client: "HORECA Solutions",
      desc: "Comprehensive food service solutions tailored for hotels, restaurants, and catering.",
      bg: "bg-[#f8f8f8]",
      img: "/generated/image-busy-professional-restaurant-kitchen-wit-1765530572910-4.webp",
      dark: false,
      full: true // Making HORECA full width to align last two items
    },
    {
      client: "Quality Assurance",
      desc: "Rigorous testing and certification ensuring food safety standards.",
      bg: "bg-[#e8e8e8]",
      img: "/generated/image-food-quality-inspector-examining-fresh-p-1765530575810-5.webp",
      dark: false
    },
    {
      client: "Supply Chain Technology",
      desc: "Real-time tracking and inventory management for seamless operations.",
      bg: "bg-[#f0f0f0]",
      img: "/generated/image-warehouse-worker-using-tablet-for-invent-1765530578022-6.webp",
      dark: false
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">We integrate sourcing, production, and distribution</span> to deliver consistent quality and freshness across the Middle East food supply chain—capturing the $850B market opportunity.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-x-6 gap-y-12">
    {#each projects as project}
      <div class="group cursor-pointer {project.full ? 'md:col-span-2' : ''}">
        <div class={`aspect-[4/3] w-full rounded-lg overflow-hidden relative ${project.bg} mb-4 ${project.full ? 'md:aspect-[2.5/1]' : ''}`}>
          {#if project.img}
             <img src={project.img} alt={project.client} class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
          {:else}
             <!-- Placeholder for logos on solid bg -->
             <div class="w-full h-full flex items-center justify-center">
                <span class={`text-2xl font-bold ${project.dark ? 'text-white' : 'text-black'}`}>{project.client} Logo</span>
             </div>
          {/if}
        </div>
        <h3 class="text-sm font-bold mb-1">{project.client}</h3>
        <p class="text-sm text-gray-600">{project.desc}</p>
      </div>
    {/each}
  </div>
</section>
