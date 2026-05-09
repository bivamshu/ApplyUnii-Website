<section class="py-24 px-8 md:px-24 bg-[#030712]">
    <div class="max-w-7xl mx-auto">
        <!-- Section Header -->
        <div class="flex flex-col md:flex-row md:items-end justify-between mb-16 gap-8">
            <div class="max-w-2xl">
                <div class="flex items-center gap-3 mb-6">
                    <div class="w-12 h-[1.5px] bg-[#00d084]"></div>
                    <span class="text-[#00d084] font-bold text-xs uppercase tracking-widest">Our Services</span>
                </div>
                <h2 class="text-5xl md:text-6xl font-bold text-white leading-tight mb-6">
                    Strategic support, <span class="text-[#00d084]">masterfully delivered</span>
                </h2>
                <p class="text-gray-400 text-lg leading-relaxed">
                    From first consultation to global enrollment, we orchestrate your journey with precision and care.
                </p>
            </div>
            
            <a href="/services" class="flex items-center gap-4 text-sm font-bold text-white hover:opacity-80 transition group shrink-0">
                <div class="w-12 h-[1px] bg-[#00d084]"></div>
                Explore All Services
            </a>
        </div>

        <!-- Services Grid -->
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            {#each [
                { 
                    id: '01',
                    title: 'Career Counselling & University Application Consultancy', 
                    desc: 'Professional Career Counselling and University Application Support',
                },
                { 
                    id: '02',
                    title: 'University application support', 
                    desc: 'End-to-end help for applications, SOPs, LORs, and document checks.',
                },
                { 
                    id: '03',
                    title: 'Visa guidance', 
                    desc: 'Prepare your visa file with clarity and reduce avoidable mistakes.',
                },
                {
                    id: '04',
                    title: 'Scholarship & finance planning',
                    desc: 'Explore scholarships and build a realistics fee + living cost plan.',
                },
                {
                    id: '05',
                    title: 'Pre-departure support',
                    desc: 'Pack right, plan right - everything you need before you fly.',
                }
            ] as service}
                <div class="relative group p-10 rounded-3xl bg-[#0f172a]/20 border border-white/5 hover:border-white/10 transition-all duration-500 overflow-hidden">
                    <!-- Background Number -->
                    <span class="absolute top-4 right-6 text-8xl font-black text-white/[0.03] group-hover:text-white/[0.07] transition-colors pointer-events-none">
                        {service.id}
                    </span>

                    <div class="relative z-10">
                        <div class="w-10 h-[2px] bg-[#00d084] mb-8"></div>
                        
                        <h3 class="text-2xl font-bold text-white mb-6 pr-10">
                            {service.title}
                        </h3>
                        
                        <p class="text-gray-400 mb-10 leading-relaxed">
                            {service.desc}
                        </p>

                        <a href="/services" class="inline-flex items-center gap-2 text-[#00d084] font-bold text-sm hover:underline">
                            Learn more 
                            <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14m-7-7 7 7-7 7"/></svg>
                        </a>
                    </div>
                </div>
            {/each}
        </div>
    </div>
</section>