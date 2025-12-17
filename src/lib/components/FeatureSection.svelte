<script>
  import AppWindow from './AppWindow.svelte';
  import Cursor from './Cursor.svelte';
  
  export let title = "";
  export let description = "";
  export let cursorName = "";
  export let cursorColor = "orange";
  export let cursorPosition = ""; // CSS classes for positioning
</script>

<section class="py-24 px-4 flex flex-col items-center text-center max-w-7xl mx-auto relative">
  <div class="mb-16 max-w-2xl mx-auto z-10 relative">
    <h2 class="text-4xl md:text-5xl font-bold tracking-tight text-gray-900 mb-6">{title}</h2>
    <p class="text-lg text-gray-500 mb-8 leading-relaxed max-w-xl mx-auto">
      {description}
    </p>
    
    <div class="flex flex-col items-center gap-2">
      <a href="#apply" class="bg-primary-600 hover:bg-primary-700 text-white text-sm font-medium px-5 py-2.5 rounded-full flex items-center gap-1.5 transition-colors shadow-sm">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" class="w-3.5 h-3.5">
          <line x1="5" y1="12" x2="19" y2="12"></line>
          <polyline points="12 5 19 12 12 19"></polyline>
        </svg>
        Join Waitlist for 2026
      </a>
      <span class="text-[10px] text-gray-400 font-medium tracking-wide uppercase">2025 Event Sold Out</span>
    </div>
    
    <div class="mt-12">
      <slot name="after-cta" />
    </div>
  </div>

  <!-- Cursor outside window -->
  {#if cursorName}
    <Cursor name={cursorName} color={cursorColor} className={cursorPosition} />
  {/if}
  
  <slot name="extra-cursors" />

  <div class="w-full max-w-5xl mx-auto px-4 md:px-8 z-0">
    <AppWindow className="w-full aspect-[16/10]">
      <slot />
    </AppWindow>
  </div>
</section>
