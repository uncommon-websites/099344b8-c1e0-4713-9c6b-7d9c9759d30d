<script lang="ts">
  const photos = [
    {
      title: "State-of-the-Art Facilities",
      desc: "Our temperature-controlled warehouses and processing centers maintain the highest food safety standards.",
      img: "/generated/image-large-modern-warehouse-interior-with-org-1765530587917-10.webp"
    },
    {
      title: "Quality at Every Step",
      desc: "From receiving to dispatch, our quality assurance team ensures every product meets our rigorous standards.",
      img: "/generated/image-quality-control-team-inspecting-fresh-pr-1765530590176-11.webp"
    },
    {
      title: "Chef-Focused Service",
      desc: "We understand kitchen operations—our team works closely with chefs to deliver exactly what they need, when they need it.",
      img: "/generated/image-professional-chef-consulting-with-food-s-1765530592450-12.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">We focus on quality, not just quantity.</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      In an industry where freshness is everything, we've built our operations around one principle: never compromise on quality. Our infrastructure, processes, and people are all aligned to deliver the consistency that HORECA professionals demand.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each photos as photo}
      <div>
        <div class="aspect-[3/4] rounded-lg overflow-hidden mb-4 bg-gray-100">
          <img src={photo.img} alt={photo.title} class="w-full h-full object-cover" />
        </div>
        <h4 class="text-xs font-bold mb-1">{photo.title}</h4>
        <p class="text-[10px] text-gray-500 leading-relaxed">{photo.desc}</p>
      </div>
    {/each}
  </div>
</section>
