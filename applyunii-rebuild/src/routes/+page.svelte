<script lang="ts">
    import Navbar from '$lib/components/Navbar.svelte';
    import Hero from '$lib/components/Hero.svelte';
    import Stats from '$lib/components/Stats.svelte';
    import Features from '$lib/components/Features.svelte';
    import Services from '$lib/components/Services.svelte';
    import Destinations from '$lib/components/Destinations.svelte';
    import TrendingCourses from '$lib/components/TrendingCourses.svelte';
    import Testimonials from '$lib/components/Testimonials.svelte';
  </script>
  
  <Navbar />
  
  <main>
      <Hero />
      <Stats />
      <Features />
      <Services />
      <Destinations />
      <TrendingCourses />
      <Testimonials />
    </main>