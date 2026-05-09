<script lang="ts">
    const courses = [
        {
            title: "MSc Advanced Computer Science with Placement Year",
            level: "Postgraduate",
            location: "UK",
            category: "IT",
            duration: "2 Years",
            intake: "September 2026",
            ielts: "Yes",
            price: "GBP16800.00",
            featured: true
        },
        {
            title: "BSc (Hons) Computer Science",
            level: "Undergraduate",
            location: "UK",
            category: "IT",
            duration: "3 Years",
            intake: "September, January",
            ielts: "6.0",
            price: null,
            featured: false
        },
        {
            title: "BSc (Hons) Information Technology",
            level: "Undergraduate",
            location: "UK",
            category: "IT",
            duration: "3 Years",
            intake: "September, January",
            ielts: "6.0",
            price: null,
            featured: false
        },
        {
            title: "Beng (Hons) Mechanical Engineering",
            level: "Undergraduate", 
            location: "UK", 
            category: "Engineering", 
            duration: "3 years", 
            intake: "September, January", 
            ielts: "6.0",
            price: null,
            featured: false
        },
        {
            title: "BSc (Hons) Nursing (Adult)",
            level: "Undergraduate", 
            location: "UK", 
            category: "Health and Medicine", 
            duration: "3 years", 
            intake: "September 2026",
            ielts: "6.5",
            price: null,
            featured: false
        },
        {
            title: "MSc Nursing (Adult) with NMC registration",
            level: "Postgraduate",
            location: "UK",
            category: "Nursing",
            duration: "2 Years",
            intake: "September 2026",
            ielts: "6.5",
            price: "GBP17500.00",
            featured: false
        }
    ];
</script>

<section class="py-24 px-8 md:px-24 bg-[#030712]">
    <div class="max-w-7xl mx-auto">
        <!-- Header -->
        <div class="flex flex-col md:flex-row md:items-end justify-between mb-16 gap-6">
            <div>
                <div class="flex items-center gap-3 mb-6">
                    <div class="w-8 h-[1.5px] bg-[#00d084]"></div>
                    <span class="text-[#00d084] font-bold text-xs uppercase tracking-widest">Trending Programmes</span>
                </div>
                <h2 class="text-5xl md:text-6xl font-bold text-white leading-tight">
                    Find the course that <span class="text-[#00d084]">defines</span> your career
                </h2>
            </div>
            <button class="px-8 py-4 rounded-xl border border-white/10 text-white font-bold text-sm hover:bg-white/5 transition-all flex items-center gap-3 shrink-0">
                Explore Catalog 
                <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2.5"><path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3" /></svg>
            </button>
        </div>

        <!-- Course Grid -->
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            {#each courses as course}
                <div class="p-8 rounded-3xl bg-[#0f172a]/20 border transition-all duration-300 flex flex-col justify-between {course.featured ? 'border-[#00d084] ring-1 ring-[#00d084]/20' : 'border-white/5 hover:border-white/10'}">
                    <div>
                        <h3 class="text-xl font-bold text-white mb-6 leading-snug {course.featured ? 'text-[#00d084]' : 'text-white'}">
                            {course.title}
                        </h3>

                        <!-- Badges -->
                        <div class="flex flex-wrap gap-2 mb-8">
                            <span class="px-3 py-1 rounded-md bg-[#00d084]/10 text-[#00d084] text-[10px] font-bold uppercase">{course.level}</span>
                            <span class="px-3 py-1 rounded-md bg-white/5 text-blue-400 text-[10px] font-bold uppercase">{course.location}</span>
                            <span class="px-3 py-1 rounded-md bg-white/5 text-gray-400 text-[10px] font-bold uppercase">{course.category}</span>
                        </div>

                        <!-- Stats/Meta -->
                        <div class="space-y-4 mb-10">
                            <div class="flex items-center gap-3 text-gray-500 text-sm">
                                <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" /></svg>
                                {course.duration}
                            </div>
                            <div class="flex items-center gap-3 text-gray-500 text-sm">
                                <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z" /></svg>
                                Intake: {course.intake}
                            </div>
                            <div class="flex items-center gap-3 text-gray-500 text-sm">
                                <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" /></svg>
                                IELTS: {course.ielts}
                            </div>
                        </div>
                    </div>

                    <div>
                        {#if course.price}
                            <div class="text-xl font-bold text-[#00d084] mb-4">
                                {course.price} <span class="text-xs text-gray-500 font-normal">/ year</span>
                            </div>
                        {/if}
                        <button class="flex items-center gap-2 text-[#00d084] font-bold text-sm hover:underline">
                            View details 
                            <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="3"><path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3" /></svg>
                        </button>
                    </div>
                </div>
            {/each}
        </div>
    </div>
</section>