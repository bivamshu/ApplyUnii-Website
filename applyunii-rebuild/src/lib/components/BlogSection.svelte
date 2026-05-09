<script lang="ts">
    const blogs = [
        {
            title: "UK Graduate Route 2026: What International Students Need to Know About the Expected...",
            category: "VISA",
            date: "9 Apr 2026",
            author: "ApplyUni",
            description: "Practical guidance from ApplyUni counsellors — updated for the latest rules and intake cycles.",
            image: "/blog-visa.png" // Placeholder for your images
        },
        {
            title: "Essential Documents for International Students Applying to UK Universities",
            category: "STRATEGY",
            date: "9 Apr 2026",
            author: "ApplyUni",
            description: "Essential Documents for International Students Applying to UK Universities",
            image: "/blog-docs.png" 
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
                    <span class="text-[#00d084] font-bold text-xs uppercase tracking-widest">Latest Insights</span>
                </div>
                <h2 class="text-5xl font-bold text-white">Guides for your journey</h2>
            </div>
            <button class="px-8 py-3 rounded-xl border border-white/10 text-white font-bold text-sm hover:bg-white/5 transition-all flex items-center gap-3 shrink-0">
                Visit Blog 
                <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2.5"><path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3" /></svg>
            </button>
        </div>

        <!-- Blog Grid -->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
            {#each blogs as blog}
                <div class="rounded-3xl bg-[#0f172a]/30 border border-white/5 overflow-hidden group hover:border-[#00d084]/30 transition-all duration-500">
                    <!-- Image Container -->
                    <div class="relative h-64 overflow-hidden">
                        <img src={blog.image} alt={blog.title} class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-700" />
                        <div class="absolute top-6 left-6">
                            <span class="px-3 py-1 rounded-md bg-[#00d084]/20 text-[#00d084] text-[10px] font-black uppercase backdrop-blur-md border border-[#00d084]/30">
                                {blog.category}
                            </span>
                        </div>
                    </div>

                    <!-- Content -->
                    <div class="p-8">
                        <div class="flex items-center gap-2 text-gray-500 text-xs mb-4">
                            <span>{blog.date}</span>
                            <span>•</span>
                            <span>{blog.author}</span>
                        </div>
                        <h3 class="text-xl font-bold text-white mb-4 leading-snug group-hover:text-[#00d084] transition-colors">
                            {blog.title}
                        </h3>
                        <p class="text-gray-500 text-sm leading-relaxed mb-8 line-clamp-2">
                            {blog.description}
                        </p>
                        <button class="flex items-center gap-2 text-[#00d084] font-bold text-sm hover:underline">
                            Read more 
                            <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="3"><path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3" /></svg>
                        </button>
                    </div>
                </div>
            {/each}
        </div>
    </div>
</section>