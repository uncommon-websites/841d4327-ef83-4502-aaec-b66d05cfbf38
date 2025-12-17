<script>
  const activities = [
    { icon: '🎤', title: 'Panels', desc: 'Future of European AI Ambition' },
    { icon: '🛠️', title: 'Workshops', desc: 'Human-AI Collaboration' },
    { icon: '🍽️', title: 'Themed Dinners', desc: 'AI & Creativity at Rathauskeller' },
    { icon: '🎨', title: 'Idea Adventures', desc: 'AI-Generated Perfume Creation' },
    { icon: '💡', title: 'Fireside Chats', desc: 'Leadership in the Age of AI' },
    { icon: '🎬', title: 'Screenings', desc: 'AI Movie with Afro Futcha' },
  ];
</script>

<div class="w-full h-full min-h-[500px] bg-gradient-to-br from-gray-50 to-white relative p-8 overflow-hidden flex items-center justify-center">
  
  <!-- Background pattern -->
  <div class="absolute inset-0 opacity-5">
    <div class="absolute inset-0" style="background-image: radial-gradient(circle at 2px 2px, rgb(0 0 0 / 0.15) 1px, transparent 0); background-size: 32px 32px;"></div>
  </div>
  
  <!-- Activity Cards -->
  <div class="grid grid-cols-3 gap-3 max-w-3xl z-10">
    {#each activities as activity}
      <div class="bg-white rounded-lg p-4 shadow-sm border border-gray-200 hover:shadow-md hover:border-primary-200 transition-all group">
        <div class="text-3xl mb-2">{activity.icon}</div>
        <h3 class="text-sm font-semibold text-gray-900 mb-1">{activity.title}</h3>
        <p class="text-xs text-gray-500 leading-tight">{activity.desc}</p>
      </div>
    {/each}
  </div>
  
  <!-- Stats floating cards -->
  <div class="absolute top-8 left-8 bg-white/90 backdrop-blur-sm rounded-xl px-4 py-3 shadow-lg border border-gray-200">
    <div class="text-xs text-gray-500 mb-1">Organizations</div>
    <div class="text-2xl font-bold text-gray-900">300+</div>
  </div>
  
  <div class="absolute bottom-8 right-8 bg-white/90 backdrop-blur-sm rounded-xl px-4 py-3 shadow-lg border border-gray-200">
    <div class="text-xs text-gray-500 mb-1">Countries</div>
    <div class="text-2xl font-bold text-gray-900">40+</div>
  </div>
  
  <!-- Connection lines visualization -->
  <svg class="absolute inset-0 w-full h-full pointer-events-none opacity-10" xmlns="http://www.w3.org/2000/svg">
    <line x1="20%" y1="30%" x2="80%" y2="70%" stroke="currentColor" stroke-width="1" class="text-primary-600"/>
    <line x1="80%" y1="30%" x2="20%" y2="70%" stroke="currentColor" stroke-width="1" class="text-primary-600"/>
    <line x1="50%" y1="20%" x2="50%" y2="80%" stroke="currentColor" stroke-width="1" class="text-primary-600"/>
  </svg>

</div>
