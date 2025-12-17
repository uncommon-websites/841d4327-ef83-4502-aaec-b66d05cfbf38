<script>
  const attendeeTypes = [
    { icon: '👔', title: 'C-Suite', percentage: '33%', desc: 'Chiefs, Presidents, Founders' },
    { icon: '🏢', title: 'Enterprise', percentage: '45%', desc: 'Technology & Innovation' },
    { icon: '🎓', title: 'Academia', percentage: '12%', desc: 'Research & Education' },
    { icon: '🏛️', title: 'Policy', percentage: '10%', desc: 'Government & Regulation' },
  ];
</script>

<div class="w-full h-full min-h-[500px] relative overflow-hidden">
  
  <!-- Elegant background with palace motif -->
  <div class="absolute inset-0 bg-gradient-to-br from-gray-900 via-gray-800 to-black"></div>
  
  <!-- Ornate pattern overlay -->
  <div class="absolute inset-0 opacity-5">
    <div class="absolute inset-0" style="background-image: repeating-linear-gradient(45deg, transparent, transparent 35px, rgba(255,255,255,.05) 35px, rgba(255,255,255,.05) 70px);"></div>
  </div>
  
  <!-- Chandelier light effect -->
  <div class="absolute top-0 left-1/2 -translate-x-1/2 w-[800px] h-[400px] bg-gradient-radial from-amber-200/20 via-transparent to-transparent blur-3xl"></div>
  
  <!-- Main content -->
  <div class="relative z-10 flex items-center justify-center h-full p-8">
    
    <!-- Attendee composition cards -->
    <div class="grid grid-cols-2 gap-4 max-w-2xl">
      {#each attendeeTypes as type}
        <div class="bg-white/10 backdrop-blur-md rounded-xl p-5 border border-white/20 hover:bg-white/15 transition-all">
          <div class="text-4xl mb-3">{type.icon}</div>
          <div class="text-white text-3xl font-bold mb-1">{type.percentage}</div>
          <div class="text-white/90 text-sm font-semibold mb-1">{type.title}</div>
          <div class="text-white/60 text-xs">{type.desc}</div>
        </div>
      {/each}
    </div>
    
  </div>
  
  <!-- Venue badge -->
  <div class="absolute top-8 left-8 bg-white/10 backdrop-blur-md rounded-xl px-4 py-3 border border-white/20">
    <div class="text-white/70 text-xs mb-1">Venue</div>
    <div class="text-white text-sm font-semibold">Hofburg Palace</div>
    <div class="text-white/60 text-xs">Vienna, Austria</div>
  </div>
  
  <!-- Application badge -->
  <div class="absolute top-8 right-8 bg-primary-600/90 backdrop-blur-md rounded-xl px-4 py-3 border border-primary-500/50">
    <div class="text-white text-xs font-semibold mb-1">🔒 Invite Only</div>
    <div class="text-white/90 text-xs">Application Required</div>
  </div>
  
  <!-- Stats at bottom -->
  <div class="absolute bottom-8 left-1/2 -translate-x-1/2 flex gap-6">
    <div class="bg-white/10 backdrop-blur-md rounded-lg px-4 py-2 border border-white/20">
      <div class="text-white text-xl font-bold">500+</div>
      <div class="text-white/70 text-xs">Attendees</div>
    </div>
    <div class="bg-white/10 backdrop-blur-md rounded-lg px-4 py-2 border border-white/20">
      <div class="text-white text-xl font-bold">300+</div>
      <div class="text-white/70 text-xs">Organizations</div>
    </div>
    <div class="bg-white/10 backdrop-blur-md rounded-lg px-4 py-2 border border-white/20">
      <div class="text-white text-xl font-bold">40+</div>
      <div class="text-white/70 text-xs">Countries</div>
    </div>
  </div>

</div>
