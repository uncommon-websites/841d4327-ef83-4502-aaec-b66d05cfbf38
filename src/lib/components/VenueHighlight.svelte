<script>
  const venueFeatures = [
    {
      icon: '🏛️',
      title: 'Historic Palace',
      description: 'Dating back to 1279, spanning over 300,000 square meters'
    },
    {
      icon: '👑',
      title: 'Habsburg Legacy',
      description: 'Seven centuries as the seat of the Habsburg Empire'
    },
    {
      icon: '🌍',
      title: 'Central Vienna',
      description: 'Easy access to the city\'s cultural offerings and attractions'
    }
  ];
</script>

<section class="py-24 px-4 max-w-7xl mx-auto">
  <div class="grid md:grid-cols-2 gap-16 items-center">
    <!-- Left: Content -->
    <div>
      <div class="inline-block bg-primary-50 text-primary-700 text-xs font-semibold px-3 py-1 rounded-full mb-6">
        VENUE
      </div>
      <h2 class="text-4xl md:text-5xl font-bold tracking-tight text-gray-900 mb-6">
        Hofburg Imperial Palace
      </h2>
      <p class="text-lg text-gray-600 mb-8 leading-relaxed">
        Experience three days of innovation and collaboration in one of the world's most prestigious venues. The Hofburg Palace combines centuries of history with modern conference facilities, creating an inspiring environment for Europe's AI leaders.
      </p>

      <div class="space-y-6">
        {#each venueFeatures as feature}
          <div class="flex gap-4">
            <div class="text-3xl flex-shrink-0">{feature.icon}</div>
            <div>
              <h3 class="font-semibold text-gray-900 mb-1">{feature.title}</h3>
              <p class="text-sm text-gray-600">{feature.description}</p>
            </div>
          </div>
        {/each}
      </div>
    </div>

    <!-- Right: Visual -->
    <div class="relative">
      <div class="aspect-[4/5] bg-gradient-to-br from-gray-900 via-gray-800 to-black rounded-3xl overflow-hidden shadow-2xl">
        <!-- Palace silhouette illustration -->
        <div class="absolute inset-0 flex items-end justify-center p-8">
          <!-- Ornate pattern -->
          <div class="absolute inset-0 opacity-10">
            <div class="absolute inset-0" style="background-image: repeating-linear-gradient(45deg, transparent, transparent 35px, rgba(255,255,255,.1) 35px, rgba(255,255,255,.1) 70px);"></div>
          </div>
          
          <!-- Palace architecture -->
          <div class="relative w-full flex items-end justify-center gap-2">
            <!-- Left tower -->
            <div class="w-16 h-48 bg-gradient-to-t from-gray-700 to-gray-600 rounded-t-lg relative">
              <div class="absolute top-0 left-1/2 -translate-x-1/2 w-8 h-8 bg-amber-600 rounded-full"></div>
            </div>
            
            <!-- Center building -->
            <div class="w-32 h-64 bg-gradient-to-t from-gray-700 to-gray-600 rounded-t-lg relative">
              <div class="absolute top-4 left-1/2 -translate-x-1/2 w-16 h-20 bg-gray-800/50 rounded-lg"></div>
              <div class="absolute top-0 left-1/2 -translate-x-1/2 w-12 h-12 bg-amber-600"></div>
            </div>
            
            <!-- Right tower -->
            <div class="w-16 h-48 bg-gradient-to-t from-gray-700 to-gray-600 rounded-t-lg relative">
              <div class="absolute top-0 left-1/2 -translate-x-1/2 w-8 h-8 bg-amber-600 rounded-full"></div>
            </div>
          </div>
        </div>

        <!-- Info badge -->
        <div class="absolute top-6 right-6 bg-white/10 backdrop-blur-md rounded-xl px-4 py-3 border border-white/20">
          <div class="text-white text-sm font-semibold">Vienna, Austria</div>
          <div class="text-white/70 text-xs">Sept 24-26, 2025</div>
        </div>
      </div>

      <!-- Floating stat -->
      <div class="absolute -bottom-6 -left-6 bg-white rounded-2xl p-6 shadow-xl border border-gray-100">
        <div class="text-3xl font-bold text-gray-900 mb-1">300,000m²</div>
        <div class="text-sm text-gray-600">Palace Complex</div>
      </div>
    </div>
  </div>
</section>
