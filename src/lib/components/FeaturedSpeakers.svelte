<script>
  const featuredSpeakers = [
    {
      name: 'Anna W. Topol',
      role: 'CTO, IBM Research',
      focus: 'AI & Quantum Computing',
      company: 'IBM'
    },
    {
      name: 'Oriol Vinyals',
      role: 'Co-Technical Lead for Gemini',
      focus: 'Research VP',
      company: 'Google DeepMind'
    },
    {
      name: 'Lukasz Kaiser',
      role: 'Researcher',
      focus: 'AI & LLMs',
      company: 'OpenAI'
    },
    {
      name: 'Swami Sivasubramanian',
      role: 'VP of Agentic AI',
      focus: 'Enterprise AI',
      company: 'Amazon Web Services'
    },
    {
      name: 'Joscha Bach',
      role: 'CEO',
      focus: 'AI & Consciousness',
      company: 'California Institute for Machine Consciousness'
    },
    {
      name: 'Hiroaki Kitano',
      role: 'President & CEO',
      focus: 'AI for Scientific Discovery',
      company: 'Sony Computer Science Laboratories'
    },
    {
      name: 'Verity Harding',
      role: 'Founder & Director',
      focus: 'AI & Geopolitics',
      company: 'University of Cambridge'
    },
    {
      name: 'Henna Virkkunen',
      role: 'Executive Vice-President',
      focus: 'Tech Sovereignty',
      company: 'European Commission'
    }
  ];
</script>

<section id="speakers" class="py-24 px-4 bg-gray-50">
  <div class="max-w-7xl mx-auto">
    <div class="text-center mb-16">
      <div class="inline-block bg-primary-50 text-primary-700 text-xs font-semibold px-3 py-1 rounded-full mb-6">
        2025 SPEAKERS
      </div>
      <h2 class="text-4xl md:text-5xl font-bold tracking-tight text-gray-900 mb-4">
        World-Class AI Leaders
      </h2>
      <p class="text-lg text-gray-500 max-w-2xl mx-auto">
        20+ talks from pioneers at OpenAI, Google DeepMind, IBM Research, AWS, and the European Commission
      </p>
    </div>

    <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6 max-w-6xl mx-auto">
      {#each featuredSpeakers as speaker}
        <div class="bg-white rounded-2xl p-6 shadow-sm border border-gray-100 hover:shadow-md transition-all group">
          <!-- Avatar with gradient -->
          <div class="w-20 h-20 rounded-full bg-gradient-to-br from-primary-400 to-primary-600 mx-auto mb-4 flex items-center justify-center text-white font-bold text-xl shadow-lg group-hover:scale-105 transition-transform">
            {speaker.name.split(' ').map(n => n[0]).join('')}
          </div>
          
          <!-- Name -->
          <h3 class="text-base font-bold text-gray-900 text-center mb-2 leading-tight">
            {speaker.name}
          </h3>
          
          <!-- Role -->
          <p class="text-sm text-gray-600 text-center mb-1 leading-tight">
            {speaker.role}
          </p>
          
          <!-- Focus -->
          <p class="text-xs text-gray-500 text-center mb-3 leading-tight">
            {speaker.focus}
          </p>
          
          <!-- Company Badge -->
          <div class="flex justify-center">
            <span class="text-[10px] font-semibold text-primary-700 bg-primary-50 px-3 py-1 rounded-full border border-primary-100">
              {speaker.company}
            </span>
          </div>
        </div>
      {/each}
    </div>

    <div class="text-center mt-12">
      <p class="text-sm text-gray-600 mb-4">
        Plus 12+ more speakers to be announced
      </p>
      <a href="#apply" class="inline-flex items-center gap-2 text-sm font-medium text-primary-600 hover:text-primary-700 transition-colors">
        View full speaker lineup
        <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"/>
        </svg>
      </a>
    </div>
  </div>
</section>
