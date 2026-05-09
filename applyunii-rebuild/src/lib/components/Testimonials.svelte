<section class="py-24 px-8 md:px-24 bg-[#030712]">
    <div class="max-w-7xl mx-auto">
        <!-- Header -->
        <div class="text-center mb-20">
            <div class="flex items-center justify-center gap-4 mb-6">
                <div class="w-10 h-[1px] bg-gray-700"></div>
                <span class="text-[#00d084] font-bold text-xs uppercase tracking-[0.3em]">Success Stories</span>
                <div class="w-10 h-[1px] bg-gray-700"></div>
            </div>
            <h2 class="text-5xl font-bold text-white">What our students say</h2>
        </div>

        <!-- Testimonials Grid -->
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            {#each [
                {
                    name: "Sagar C.",
                    course: "Mechanical Engineering",
                    country: "UK",
                    quote: "I applied for my course through ApplyUnii from inside the UK. The process was smooth, documentation was handled very professionally, and the team was always easy to contact whenever I needed help. I am very satisfied with their support.",
                    image: "https://i.pravatar.cc/150?u=sagar"
                }
            ] as testimonial}
                <div class="p-10 rounded-3xl bg-[#0f172a]/20 border border-white/5 flex flex-col justify-between">
                    <div>
                        <!-- Stars -->
                        <div class="flex gap-1 mb-6">
                            {#each Array(5) as _}
                                <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4 text-yellow-500 fill-current" viewBox="0 0 24 24"><path d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"/></svg>
                            {/each}
                        </div>
                        
                        <p class="text-gray-400 italic leading-relaxed mb-10">
                            "{testimonial.quote}"
                        </p>
                    </div>

                    <div class="flex items-center gap-4 pt-8 border-t border-white/5">
                        <img src={testimonial.image} alt={testimonial.name} class="w-12 h-12 rounded-full object-cover border border-[#00d084]/30" />
                        <div>
                            <h4 class="text-white font-bold">{testimonial.name}</h4>
                            <p class="text-gray-500 text-xs">{testimonial.course} · {testimonial.country}</p>
                        </div>
                    </div>
                </div>
            {/each}
        </div>
    </div>
</section>