<script lang="ts">
  const stats = [
    {
      label: "5,000+ Clients",
      desc: "From boutique restaurants to five-star hotels, we serve over 5,000 HORECA clients across Bahrain and the wider Middle East. Our diverse client base trusts us for consistent quality and reliable delivery, making us the preferred partner for food service professionals.",
      img: "https://images.unsplash.com/photo-1414235077428-338989a2e8c0?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "$850B Market",
      desc: "The Middle East food distribution market represents an $850 billion opportunity. Through vertical integration and strategic expansion, we're positioned to capture significant market share while maintaining the quality and service standards that set us apart.",
      img: "https://images.unsplash.com/photo-1579621970563-ebec7560ff3e?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "Bahrain HQ",
      desc: "Headquartered in Bahrain, our strategic location serves as the perfect hub for Middle East operations. Our state-of-the-art facilities include temperature-controlled warehouses, processing centers, and a fleet of refrigerated vehicles ensuring freshness at every step.",
      img: "https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "Same-Day Delivery",
      desc: "Our same-day delivery guarantee addresses the biggest pain point in HORECA operations—unreliable freshness. With optimized logistics and real-time tracking, we ensure ingredients arrive fresh and on time, every time. No compromises on quality.",
      img: "https://images.unsplash.com/photo-1566576721346-d4a3b4eaeb55?auto=format&fit=crop&q=80&w=200"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      The numbers tell our story. Here's a snapshot of our reach, market position, and the commitments that drive our success.
    </p>
  </div>

  <div class="space-y-16">
    {#each stats as stat}
      <div class="flex flex-col md:flex-row md:items-start justify-between gap-8 border-b border-gray-100 pb-16 last:border-0">
        <h3 class="text-2xl md:text-4xl font-medium w-full md:w-1/3">{stat.label}</h3>
        <div class="w-full md:w-1/3">
           <p class="text-xs leading-relaxed text-gray-500">{stat.desc}</p>
        </div>
        <div class="w-full md:w-1/6 flex justify-end">
           <img src={stat.img} alt={stat.label} class="w-20 h-20 object-cover rounded bg-gray-100" />
        </div>
      </div>
    {/each}
  </div>
</section>
