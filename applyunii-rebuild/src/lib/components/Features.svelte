<section class="py-24 px-8 md:px-24 bg-[#0b1120]">
    <div class="max-w-7xl mx-auto">
        <div class="flex flex-col md:flex-row md:items-end justify-between mb-16 gap-6">
            <div class="space-y-4">
                <div class="flex items-center gap-3">
                    <div class="w-12 h-[1px] bg-[#00d084]"></div>
                    <span class="text-[#00d084] font-bold text-xs uppercase tracking-[0.2em]">Why Choose Us</span>
                </div>
                <h2 class="text-4xl md:text-6xl font-bold text-white leading-tight">
                    Guidance you can <span class="text-[#00d084]">depend on</span>
                </h2>
            </div>
            
            <a href="/services" class="flex items-center gap-4 text-sm font-bold text-gray-300 hover:text-white transition group">
                See More 
                <div class="w-12 h-[1px] bg-gray-600 group-hover:bg-[#00d084] transition-colors"></div>
            </a>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
            {#each [
                { 
                    title: 'Expert Education Counselling', 
                    desc: 'Our team provides professional guidance from a British Council Certified Counsellor, ensuring student...',
                    icon: '🎓' 
                },
                { 
                    title: 'Complete Application Support', 
                    desc: 'We assist students throughout the entire university application process, from preparing documents to...',
                    icon: '📄' 
                },
                { 
                    title: 'Visa Application Guidance', 
                    desc: 'Our experienced team helps students prepare strong visa applications, ensuring all requirements are properly...',
                    icon: '🛂' 
                },
                { 
                    title: 'Global Study Opportunities', 
                    desc: 'We connect students with reputable international universities, helping them access quality education and global...',
                    icon: '🌎' 
                }
            ] as feature}
                <div class="group p-8 rounded-2xl bg-[#0f172a]/40 border border-white/5 hover:border-[#00d084]/30 transition-all duration-500 hover:-translate-y-2">
                    <div class="w-14 h-14 bg-white/5 rounded-2xl flex items-center justify-center text-2xl mb-8 group-hover:bg-[#00d084]/20 group-hover:scale-110 transition-all duration-500">
                        {feature.icon}
                    </div>
                    
                    <h3 class="text-xl font-bold text-white mb-4 leading-snug">
                        {feature.title}
                    </h3>
                    
                    <p class="text-gray-400 text-sm leading-relaxed line-clamp-3">
                        {feature.desc}
                    </p>
                </div>
            {/each}
        </div>
    </div>
</section>