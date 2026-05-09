<section class="py-24 px-8 md:px bg-[#030712]">
    <div class="max-w-7xl mx-auto">
        <!--Centered Header-->
        <div class="text-center mb-20">
            <div class="felx items-center justify-center gap-4 mb-6">
                <div class="w-10 h-[1px] bg-gray-700"></div>
                <span class="text-[#00d084] font-bold text-xs uppercase tracking-[0.3em]">Study Destinations</span>
                <div class="w-10  h-[1px] bg-gray-700"></div>
            </div>
            <h2 class="text-5xl md:text-6xl font-bold text-white">
                Where your <span class="text-[#00d084]">global future </span>begins
            </h2>
        </div>

        <!--Desitnations grid-->
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6">
            {#each [
                {name: 'United Kingdom', flag: '🇬🇧'},
                {name: 'Australlia', flag: '🇦🇺'},
                {name: 'Canada', flag: '🇨🇦'},
                {name: 'New Zealand', flag: '🇳🇿'},
                {name: 'USA', flag: '🇺🇸'},
                {name: 'Germany', flag: '🇩🇪'}
            ] as country}
                <div class="group p-8 rounded-2xl bg-[#0f172a]/20 border border-white/5 hover:border-[#00d084]/20 transition-all duration-500 hover-bg-[#0f172a]/40">
                    <div class="text-4xl mb-6 grayscale group-hover:grayscale-0 transition-all duration-500 transform group-hover:scale-110 origin-left">
                        {country.flag}
                    </div>
                        
                    <h3 class="text-xl font-bold text-white mb-3">
                        {country.name}
                    </h3>
        
                    <p class="text-gray-400 text-sm leading-relaxed">
                        Top inviersities, strong employability, and great student support.
                    </p>
                </div>
            {/each}  
        </div>
    </div>
</section>