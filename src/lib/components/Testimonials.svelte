<script>
  const testimonials = [
    {
      quote: "The TEDAI Vienna Conference was one of the best conferences I've attended in recent years. Each day was meticulously planned, the location was perfect, and the participants were incredibly engaging.",
      author: "Sebastian Krüger",
      role: "CEO, Ray Sono AG"
    },
    {
      quote: "TEDAI Vienna 2024 was an inspiring platform bringing together leading voices in AI, innovation, and sustainability. The ideas and collaborations born here have the potential to reshape industries.",
      author: "Jason Slater",
      role: "Chief Digital and Innovation Officer, UNIDO"
    },
    {
      quote: "TED AI made a terrific job in offering me the quality content I was searching for in the field of AI for a long time through its fact-checked, and brilliantly-curated program.",
      author: "Gabriella Chihan Stanley",
      role: "Co-founder & CCO, vrisch XR"
    }
  ];
</script>

<section class="py-24 px-4 max-w-7xl mx-auto">
  <div class="text-center mb-16">
    <h2 class="text-4xl md:text-5xl font-bold tracking-tight text-gray-900 mb-4">
      What Attendees Say
    </h2>
    <p class="text-lg text-gray-500 max-w-2xl mx-auto">
      Hear from executives and leaders who experienced TEDAI Vienna
    </p>
  </div>

  <div class="grid md:grid-cols-3 gap-8 max-w-6xl mx-auto">
    {#each testimonials as testimonial}
      <div class="bg-white rounded-2xl p-8 shadow-sm border border-gray-100 hover:shadow-md transition-shadow">
        <div class="mb-6">
          <svg class="w-8 h-8 text-primary-600 opacity-50" fill="currentColor" viewBox="0 0 24 24">
            <path d="M14.017 21v-7.391c0-5.704 3.731-9.57 8.983-10.609l.995 2.151c-2.432.917-3.995 3.638-3.995 5.849h4v10h-9.983zm-14.017 0v-7.391c0-5.704 3.748-9.57 9-10.609l.996 2.151c-2.433.917-3.996 3.638-3.996 5.849h3.983v10h-9.983z"/>
          </svg>
        </div>
        <p class="text-gray-700 mb-6 leading-relaxed">
          "{testimonial.quote}"
        </p>
        <div class="border-t border-gray-100 pt-4">
          <div class="font-semibold text-gray-900">{testimonial.author}</div>
          <div class="text-sm text-gray-500">{testimonial.role}</div>
        </div>
      </div>
    {/each}
  </div>
</section>
