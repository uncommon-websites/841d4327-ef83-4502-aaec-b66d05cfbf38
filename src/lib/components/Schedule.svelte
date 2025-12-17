<script>
  const schedule = [
    {
      day: 'Day 1',
      date: 'Wednesday, September 24',
      events: [
        { time: '9:30 AM - 3:00 PM', title: 'TEDx Organizer Workshop', location: 'External Location' },
        { time: '1:00 PM - 5:00 PM', title: 'Check-in & Community Meet-Ups', location: 'Hofburg Palace' },
        { time: '8:00 PM - 11:30 PM', title: 'Opening Gala', location: 'Creative Black Tie' }
      ]
    },
    {
      day: 'Day 2',
      date: 'Thursday, September 25',
      events: [
        { time: '9:00 AM - 10:00 AM', title: 'Wellness Breakfast', location: 'Hofburg Palace' },
        { time: '10:00 AM - 5:30 PM', title: 'Discovery Sessions', location: 'Panels, Workshops & Adventures' },
        { time: '5:30 PM - 9:00 PM', title: 'Themed AI Dinners', location: 'Rathauskeller Restaurant' }
      ]
    },
    {
      day: 'Day 3',
      date: 'Friday, September 26',
      events: [
        { time: '8:30 AM - 9:30 AM', title: 'Brunch and Beats with DJ', location: 'Hofburg Palace' },
        { time: '9:30 AM - 7:30 PM', title: 'TED Talks', location: '20+ Curated Sessions' },
        { time: '7:30 PM - Midnight', title: 'Afterparty', location: 'Celebration' }
      ]
    }
  ];
</script>

<section id="about" class="py-24 px-4 max-w-7xl mx-auto">
  <div class="text-center mb-16">
    <div class="inline-block bg-primary-50 text-primary-700 text-xs font-semibold px-3 py-1 rounded-full mb-6">
      SCHEDULE
    </div>
    <h2 class="text-4xl md:text-5xl font-bold tracking-tight text-gray-900 mb-4">
      Three Days of Innovation
    </h2>
    <p class="text-lg text-gray-500 max-w-2xl mx-auto">
      From opening gala to closing afterparty, every moment is designed for connection and inspiration
    </p>
  </div>

  <div class="grid md:grid-cols-3 gap-8 max-w-6xl mx-auto">
    {#each schedule as day}
      <div class="bg-white rounded-2xl p-8 shadow-sm border border-gray-100 hover:shadow-md transition-shadow">
        <div class="mb-6">
          <div class="text-primary-600 font-bold text-sm mb-1">{day.day}</div>
          <div class="text-gray-900 font-semibold text-lg">{day.date}</div>
        </div>

        <div class="space-y-6">
          {#each day.events as event}
            <div class="border-l-2 border-primary-200 pl-4">
              <div class="text-xs text-gray-500 font-medium mb-1">{event.time}</div>
              <div class="font-semibold text-gray-900 mb-1">{event.title}</div>
              <div class="text-sm text-gray-600">{event.location}</div>
            </div>
          {/each}
        </div>
      </div>
    {/each}
  </div>

  <div class="text-center mt-12">
    <p class="text-sm text-gray-500">
      All conference passes include access to all three days, meals, and networking events
    </p>
  </div>
</section>
