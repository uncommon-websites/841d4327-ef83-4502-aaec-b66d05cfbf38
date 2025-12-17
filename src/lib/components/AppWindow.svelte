<script>
  export let className = "";
</script>

<div class="bg-white rounded-3xl shadow-sm border border-gray-100 overflow-hidden relative {className}">
  <!-- Top Bar -->
  <div class="h-14 border-b border-gray-100 flex items-center justify-between px-4">
    <!-- Left: TEDAI Vienna branding -->
    <div class="flex items-center gap-2">
      <div class="w-8 h-8 bg-primary-600 rounded-full flex items-center justify-center">
        <span class="text-white font-bold text-[8px] text-center leading-tight">TED<br/>AI</span>
      </div>
      <span class="text-[13px] font-semibold text-gray-900">TEDAI Vienna</span>
    </div>

    <!-- Right: Conference info -->
    <div class="flex items-center gap-3">
      <div class="text-[11px] text-gray-500 font-medium">
        Sept 24-26, 2025
      </div>
      <div class="w-px h-4 bg-gray-200"></div>
      <div class="text-[11px] text-gray-500 font-medium">
        Hofburg Palace
      </div>
    </div>
  </div>

  <!-- Content Slot -->
  <div class="relative min-h-[400px] bg-white">
    <slot />
  </div>

  <!-- Bottom badge -->
  <div class="absolute bottom-4 left-4 bg-white/90 backdrop-blur-sm border border-gray-200 rounded-full shadow-sm px-3 py-1.5">
    <span class="text-[10px] font-semibold text-gray-700">2025 Event</span>
  </div>
</div>
