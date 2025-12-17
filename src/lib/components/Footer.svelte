<script>
  import { ArrowRight } from 'lucide-svelte';
</script>

<footer class="py-32 px-4 flex flex-col items-center text-center">
  <div class="w-16 h-16 bg-primary-600 rounded-full flex items-center justify-center text-white mb-8 shadow-lg rotate-[-6deg]">
    <span class="font-bold text-sm">TED<br/>AI</span>
  </div>
  
  <h2 class="text-4xl md:text-5xl font-bold tracking-tight text-gray-900 mb-10 max-w-xl leading-tight">
    Join Europe's Premier<br/>
    AI Conference in 2026
  </h2>
  
  <a href="#apply" class="bg-primary-600 hover:bg-primary-700 text-white text-sm font-medium px-6 py-3 rounded-full flex items-center gap-2 transition-colors shadow-md mb-16">
    Apply for 2026
    <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" class="w-3.5 h-3.5">
       <line x1="5" y1="12" x2="19" y2="12"></line>
       <polyline points="12 5 19 12 12 19"></polyline>
    </svg>
  </a>
  
  <div class="flex flex-col items-center gap-6 w-full">
    <div class="flex items-center gap-6 text-sm text-gray-500 font-medium">
      <a href="https://www.instagram.com/tedai.vienna/" target="_blank" rel="noopener" class="hover:text-gray-900 transition-colors">Instagram</a>
      <div class="w-1 h-1 bg-gray-300 rounded-full"></div>
      <a href="https://www.linkedin.com/company/tedai-vienna/" target="_blank" rel="noopener" class="hover:text-gray-900 transition-colors">LinkedIn</a>
      <div class="w-1 h-1 bg-gray-300 rounded-full"></div>
      <a href="https://tedaivienna.com" target="_blank" rel="noopener" class="hover:text-gray-900 transition-colors">Official Site</a>
    </div>
    
    <div class="flex items-center gap-6 text-[11px] text-gray-400">
      <a href="/terms" class="hover:text-gray-600 transition-colors">Terms of service</a>
      <div class="w-1 h-1 bg-gray-300 rounded-full"></div>
      <a href="/privacy" class="hover:text-gray-600 transition-colors">Privacy Policy</a>
    </div>
    
    <div class="text-xs text-gray-400 mt-4">
      © 2025 TEDAI Vienna. Curated by Dr. Alina Nikolaou in collaboration with TED.
    </div>
  </div>
</footer>
