<script lang="ts">
  // Key clients and partners in Bahrain HORECA market
  const logos = [
    "Four Seasons",
    "Ritz-Carlton",
    "Gulf Hotel",
    "The Domain",
    "Coral Bay"
  ];
</script>

<section class="relative min-h-screen flex flex-col justify-end pb-20 px-6 md:px-12 bg-gradient-to-b from-[#1a1a1a] via-[#2a2a2a] to-white text-[#1a1a1a]">
  <!-- Gradient overlay/background handling -->
  <div class="absolute inset-0 z-[-1] bg-[linear-gradient(180deg,#0a0a0a_0%,#1a1a1a_30%,#f5f5f5_80%,#fff_100%)]"></div>

  <div class="max-w-4xl mb-32 pt-40">
    <h1 class="text-3xl md:text-5xl font-medium leading-[1.15] tracking-tight text-white">
      Integrated Food Supply Chain Solutions for the Middle East. <span class="text-gray-400">From farm to table, we deliver consistent quality through vertical integration—serving 5,000+ HORECA clients with same-day freshness guarantees.</span>
    </h1>
  </div>

  <div class="border-t border-gray-300 pt-8 flex flex-wrap gap-8 md:gap-16 items-center opacity-60 grayscale">
    {#each logos as logo}
      <div class="h-8 flex items-center justify-center font-bold text-xl text-gray-600">{logo}</div>
    {/each}
  </div>
</section>
