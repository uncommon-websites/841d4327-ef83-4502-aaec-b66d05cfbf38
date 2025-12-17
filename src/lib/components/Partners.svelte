<script>
  const partners = [
    { name: 'PwC', tier: 'Flagship Partner' },
    { name: 'JetBrains', tier: 'Lead Partner' },
    { name: 'SHIFT', tier: 'Lead Partner' },
    { name: 'City of Vienna', tier: 'Smart Cities Partner' },
    { name: 'Vienna Business Agency', tier: 'Growth Partner' },
    { name: 'Hotel Sacher', tier: 'Hospitality Partner' }
  ];
</script>

<section class="py-24 px-4 bg-gray-50">
  <div class="max-w-7xl mx-auto text-center">
    <h2 class="text-3xl md:text-4xl font-bold tracking-tight text-gray-900 mb-4">
      Trusted by Leading Organizations
    </h2>
    <p class="text-lg text-gray-500 mb-16 max-w-2xl mx-auto">
      TEDAI Vienna partners with organizations committed to building a brighter technological future
    </p>

    <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-8 items-center">
      {#each partners as partner}
        <div class="flex flex-col items-center gap-2">
          <div class="w-full aspect-square bg-white rounded-xl shadow-sm border border-gray-200 flex items-center justify-center p-6 hover:shadow-md transition-shadow">
            <div class="text-center">
              <div class="font-bold text-gray-900 text-lg mb-1">{partner.name}</div>
              <div class="text-[10px] text-gray-500 font-medium uppercase tracking-wide">{partner.tier}</div>
            </div>
          </div>
        </div>
      {/each}
    </div>

    <div class="mt-16">
      <a href="#partner" class="text-sm font-medium text-primary-600 hover:text-primary-700 transition-colors">
        Interested in partnering? Get in touch →
      </a>
    </div>
  </div>
</section>
