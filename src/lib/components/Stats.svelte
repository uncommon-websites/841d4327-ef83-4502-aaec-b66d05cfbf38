<script>
  const stats = [
    { value: '500+', label: 'Attendees', description: 'AI leaders and innovators' },
    { value: '40+', label: 'Countries', description: 'Global representation' },
    { value: '300+', label: 'Organizations', description: 'Unique companies' },
    { value: '33%', label: 'C-Suite', description: 'Executive-level positions' },
    { value: '20+', label: 'TED Talks', description: 'Curated presentations' },
    { value: '3 Days', label: 'Full Program', description: 'Immersive experience' }
  ];
</script>

<section class="py-24 px-4 bg-gradient-to-b from-white to-gray-50">
  <div class="max-w-7xl mx-auto">
    <div class="text-center mb-16">
      <h2 class="text-3xl md:text-4xl font-bold tracking-tight text-gray-900 mb-4">
        TEDAI Vienna by the Numbers
      </h2>
      <p class="text-lg text-gray-500 max-w-2xl mx-auto">
        Join Europe's most selective AI conference
      </p>
    </div>

    <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-8 max-w-6xl mx-auto">
      {#each stats as stat}
        <div class="text-center">
          <div class="text-4xl md:text-5xl font-bold text-gray-900 mb-2">
            {stat.value}
          </div>
          <div class="text-sm font-semibold text-gray-900 mb-1">
            {stat.label}
          </div>
          <div class="text-xs text-gray-500">
            {stat.description}
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>
