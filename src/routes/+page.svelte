<script>
  import Navbar from '$lib/components/Navbar.svelte';
  import Hero from '$lib/components/Hero.svelte';
  import FeatureSection from '$lib/components/FeatureSection.svelte';
  import IntuitiveWindowContent from '$lib/components/IntuitiveWindowContent.svelte';
  import SmartWindowContent from '$lib/components/SmartWindowContent.svelte';
  import SafeWindowContent from '$lib/components/SafeWindowContent.svelte';
  import VenueHighlight from '$lib/components/VenueHighlight.svelte';
  import FeaturedSpeakers from '$lib/components/FeaturedSpeakers.svelte';
  import Stats from '$lib/components/Stats.svelte';
  import Schedule from '$lib/components/Schedule.svelte';
  import Testimonials from '$lib/components/Testimonials.svelte';
  import Partners from '$lib/components/Partners.svelte';
  import FinalCTA from '$lib/components/FinalCTA.svelte';
  import Footer from '$lib/components/Footer.svelte';
</script>

<svelte:head>
  <title>TEDAI Vienna 2025 | Europe's Premier AI Conference</title>
  <meta name="description" content="Join 500+ AI leaders from 40+ countries at TEDAI Vienna. Three days of curated TED Talks, workshops, and collaboration at the historic Hofburg Imperial Palace. September 24-26, 2025." />
  <meta property="og:title" content="TEDAI Vienna 2025 | Europe's Premier AI Conference" />
  <meta property="og:description" content="Join 500+ AI leaders from 40+ countries at TEDAI Vienna. Three days of curated TED Talks, workshops, and collaboration at the historic Hofburg Imperial Palace." />
  <meta property="og:type" content="website" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="TEDAI Vienna 2025 | Europe's Premier AI Conference" />
  <meta name="twitter:description" content="Join 500+ AI leaders from 40+ countries at TEDAI Vienna. September 24-26, 2025 at Hofburg Imperial Palace." />
</svelte:head>

<Navbar />

<main class="overflow-hidden">
  <Hero />

  <FeatureSection 
    title="Curated Excellence" 
    description="20+ TED Talks from world-class speakers including leaders from OpenAI, Google DeepMind, IBM Research, and the European Commission. Every talk is fact-checked and curated to TED's highest standards."
  >
    <IntuitiveWindowContent />
  </FeatureSection>

  <FeatureSection 
    title="Cross-Industry Collaboration" 
    description="Connect with 500+ AI leaders from 40+ countries and 300+ organizations. Engage in panels, workshops, themed dinners, and idea adventures designed to foster meaningful collaboration."
  >
    <SmartWindowContent />
  </FeatureSection>

  <FeatureSection 
    title="Exclusive Community" 
    description="Application-only, invite-only conference at Vienna's historic Hofburg Imperial Palace. One in three attendees holds executive-level positions, creating an unparalleled networking environment."
  >
    <SafeWindowContent />
  </FeatureSection>

  <FeaturedSpeakers />

  <Stats />

  <VenueHighlight />

  <Schedule />

  <Testimonials />

  <Partners />

  <FinalCTA />

  <Footer />
</main>

