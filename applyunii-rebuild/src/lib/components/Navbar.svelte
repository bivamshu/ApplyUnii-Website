<script lang="ts">
    import { onMount } from 'svelte';
    let scrolled = false;

    onMount(() => {
        const handleScroll = () => {
            scrolled = window.scrollY > 20;
        };
        window.addEventListener('scroll', handleScroll);
        // Fixed typo 'Scroll' -> 'scroll'
        return () => window.removeEventListener('scroll', handleScroll);
    });
</script>

<nav class="fixed top-0 left-0 w-full z-[100] px-10 transition-all duration-500 flex items-center justify-between
    {scrolled ? 'bg-[#0b1120]/90 backdrop-blur-md py-4' : 'bg-transparent py-8'}">
    
    <div class="flex items-center gap-2 cursor-pointer">
        <div class="w-10 h-10 flex items-center justify-center">
            <svg viewBox="0 0 40 40" class="w-full h-full text-white fill-current">
                <path d="M20 5C11.7 5 5 11.7 5 20s6.7 15 15 15 15-6.7 15-15S28.3 5 20 5zm0 2c7.2 0 13 5.8 13 13s-5.8 13-13 13-13-5.8-13-13 5.8-13 13-13z"/>
            </svg>
        </div>
        <span class="text-xl font-bold tracking-tight text-white">applyunii</span>
    </div>

    <div class="hidden lg:flex items-center gap-8">
        {#each ['Home','About Us', 'Courses', 'Testimonials', 'Blogs', 'Our Teams', 'Contact Us'] as link}
        <a 
            href ="#{link.toLowerCase().replace(' ', '-')}"
            class="text-sm font-medium text-gray-300 hover:text-white transition-colors duration-200">
            {link}
        </a>
        {/each}
    </div>

    <div class="flex items-center">
        <button class="bg-[#00a96e] hover:bg-[#008f5d] text-white px-6 py-2.5 rounded-full text-sm font-semibold flex items-center gap-2 transition-all active:scale-95">
            Book Appointment <span class="text-lg">→</span>
        </button>
    </div>
</nav>