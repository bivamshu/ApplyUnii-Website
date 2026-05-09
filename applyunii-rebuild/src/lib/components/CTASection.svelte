<script lang="ts">
    let formData = {
        name: '',
        email: '',
        country: '',
        course: ''
    };

    const handleSubmit = () => {
        console.log("Form submitted:", formData);
        // Logic for handling lead submission goes here
    };
</script>

<section class="py-24 px-8 md:px-24 bg-[#030712]">
    <div class="max-w-7xl mx-auto">
        <div class="bg-gradient-to-br from-[#0f172a] to-[#030712] rounded-[40px] p-12 md:p-20 border border-white/5 relative overflow-hidden">
            <!-- Background Glow Decor -->
            <div class="absolute -top-24 -right-24 w-96 h-96 bg-[#00d084]/10 blur-[100px] rounded-full"></div>
            
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center relative z-10">
                <!-- Text Content -->
                <div>
                    <h2 class="text-5xl md:text-6xl font-bold text-white leading-tight mb-8">
                        Ready to take the <br />
                        <span class="text-[#00d084]">first step?</span>
                    </h2>
                    <p class="text-gray-400 text-lg mb-10 max-w-md leading-relaxed">
                        Join thousands of students who achieved their study abroad dreams with our expert guidance.
                    </p>
                    
                    <div class="flex flex-wrap gap-6">
                        <div class="flex items-center gap-3">
                            <div class="w-6 h-6 rounded-md bg-[#00d084]/20 flex items-center justify-center">
                                <svg class="w-4 h-4 text-[#00d084]" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"/></svg>
                            </div>
                            <span class="text-white font-medium">Free Counselling</span>
                        </div>
                        <div class="flex items-center gap-3">
                            <div class="w-6 h-6 rounded-md bg-[#00d084]/20 flex items-center justify-center">
                                <svg class="w-4 h-4 text-[#00d084]" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"/></svg>
                            </div>
                            <span class="text-white font-medium">Quick Support</span>
                        </div>
                    </div>
                </div>

                <!-- Form Card -->
                <div class="bg-[#1e293b]/30 p-10 rounded-3xl border border-white/5 backdrop-blur-sm">
                    <form on:submit|preventDefault={handleSubmit} class="space-y-6">
                        <div>
                            <label class="block text-white text-sm font-bold mb-3" for="name">Full name</label>
                            <input bind:value={formData.name} id="name" type="text" class="w-full bg-[#0f172a]/50 border border-white/10 rounded-xl px-5 py-4 text-white focus:border-[#00d084]/50 outline-none transition-all" />
                        </div>
                        
                        <div>
                            <label class="block text-white text-sm font-bold mb-3" for="email">Email</label>
                            <input bind:value={formData.email} id="email" type="email" class="w-full bg-[#0f172a]/50 border border-white/10 rounded-xl px-5 py-4 text-white focus:border-[#00d084]/50 outline-none transition-all" />
                        </div>

                        <div>
                            <label class="block text-white text-sm font-bold mb-3" for="country">Interested country</label>
                            <select bind:value={formData.country} id="country" class="w-full bg-[#0f172a]/50 border border-white/10 rounded-xl px-5 py-4 text-gray-400 focus:border-[#00d084]/50 outline-none transition-all appearance-none">
                                <option value="" disabled selected>Select Country</option>
                                <option value="UK">United Kingdom</option>
                                <option value="USA">USA</option>
                                <option value="Canada">Canada</option>
                            </select>
                        </div>

                        <div>
                            <label class="block text-white text-sm font-bold mb-3" for="course">Course interest (optional)</label>
                            <input bind:value={formData.course} id="course" type="text" placeholder="e.g. MSc Data Science" class="w-full bg-[#0f172a]/50 border border-white/10 rounded-xl px-5 py-4 text-white placeholder-gray-600 focus:border-[#00d084]/50 outline-none transition-all" />
                        </div>

                        <button type="submit" class="w-full bg-white text-[#030712] font-black py-5 rounded-xl hover:bg-gray-100 transition-colors mt-4">
                            Get matched — we'll reach out
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </div>
</section>