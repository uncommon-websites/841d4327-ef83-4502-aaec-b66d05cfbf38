<script>
  const speakers = [
    { name: 'Anna W. Topol', role: 'CTO, IBM Research', company: 'IBM' },
    { name: 'Joscha Bach', role: 'CEO, California Institute', company: 'CIMC' },
    { name: 'Lukasz Kaiser', role: 'Researcher', company: 'OpenAI' },
    { name: 'Oriol Vinyals', role: 'Research VP', company: 'DeepMind' },
    { name: 'Swami Sivasubramanian', role: 'VP Agentic AI', company: 'AWS' },
    { name: 'Hiroaki Kitano', role: 'President & CEO', company: 'Sony CSL' },
  ];
</script>

<div class="w-full h-full min-h-[500px] bg-gradient-to-br from-gray-50 to-gray-100 relative p-8 flex items-center justify-center">
  
  <!-- Speaker Cards Grid -->
  <div class="grid grid-cols-3 gap-4 max-w-4xl">
    {#each speakers as speaker, i}
      <div class="bg-white rounded-xl p-4 shadow-sm border border-gray-200 hover:shadow-md transition-shadow">
        <!-- Avatar -->
        <div class="w-16 h-16 rounded-full bg-gradient-to-br from-primary-400 to-primary-600 mx-auto mb-3 flex items-center justify-center text-white font-bold text-lg">
          {speaker.name.split(' ').map(n => n[0]).join('')}
        </div>
        
        <!-- Name -->
        <h3 class="text-sm font-semibold text-gray-900 text-center mb-1 leading-tight">{speaker.name}</h3>
        
        <!-- Role -->
        <p class="text-xs text-gray-500 text-center leading-tight mb-1">{speaker.role}</p>
        
        <!-- Company Badge -->
        <div class="flex justify-center mt-2">
          <span class="text-[10px] font-medium text-primary-600 bg-primary-50 px-2 py-0.5 rounded-full">{speaker.company}</span>
        </div>
      </div>
    {/each}
  </div>
  
  <!-- Floating badge -->
  <div class="absolute top-8 right-8 bg-white rounded-xl px-4 py-3 shadow-lg border border-gray-200">
    <div class="text-xs text-gray-500 mb-1">Featured Speakers</div>
    <div class="text-2xl font-bold text-gray-900">20+</div>
  </div>
  
  <!-- TED Circle Logo -->
  <div class="absolute bottom-8 left-8 w-12 h-12 rounded-full bg-primary-600 flex items-center justify-center">
    <span class="text-white font-bold text-[10px] text-center leading-tight">TED<br/>AI</span>
  </div>

</div>
