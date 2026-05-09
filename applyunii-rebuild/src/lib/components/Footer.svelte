<footer class="bg-[#020617] pt-24 pb-12 px-8 md:px-24 border-t border-white/5">
    <div class="max-w-7xl mx-auto">
        <!-- Changed to items-start to keep cards aligned at the top -->
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-12 mb-20 items-start">
            
            <!-- Brand Column -->
            <div class="space-y-8">
                <!-- Ensure your logo path is correct -->
                <img src="/logo.png" alt="ApplyUni Logo" class="h-10" />
                <p class="text-gray-400 text-sm leading-relaxed max-w-xs">
                    <span class="font-bold text-white">ApplyUnii</span> is an international education consultancy platform operated under <span class="font-bold text-white">Everest Recruitment and Services Ltd.</span> The platform is dedicated to supporting students who wish to pursue higher...
                </p>
                <div class="flex gap-4">
                    <!-- Added actual FontAwesome classes -->
                    <a href="/" class="w-10 h-10 rounded-xl bg-[#0f172a] border border-white/5 flex items-center justify-center text-gray-400 hover:text-[#00d084] hover:border-[#00d084]/30 transition-all">
                        <i class="fa-brands fa-facebook-f"></i>
                    </a>
                    <a href="/" class="w-10 h-10 rounded-xl bg-[#0f172a] border border-white/5 flex items-center justify-center text-gray-400 hover:text-[#00d084] hover:border-[#00d084]/30 transition-all">
                        <i class="fa-brands fa-instagram"></i>
                    </a>
                    <a href="/" class="w-10 h-10 rounded-xl bg-[#0f172a] border border-white/5 flex items-center justify-center text-gray-400 hover:text-[#00d084] hover:border-[#00d084]/30 transition-all">
                        <i class="fa-brands fa-linkedin-in"></i>
                    </a>
                </div>
            </div>

            <!-- Quick Links -->
            <div>
                <h4 class="text-white font-bold uppercase tracking-widest text-[10px] mb-8">Quick Links</h4>
                <ul class="space-y-4">
                    {#each ['Home', 'About Us', 'Services', 'Courses', 'Our Team', 'Blog', 'Contact'] as link}
                        <li>
                            <a href="/" class="text-gray-400 hover:text-white text-sm transition-colors">{link}</a>
                        </li>
                    {/each}
                </ul>
            </div>

            <!-- Office UK -->
            <div>
                <h4 class="text-white font-bold uppercase tracking-widest text-[10px] mb-8">Our Offices</h4>
                <div class="p-6 rounded-2xl bg-[#0f172a]/50 border border-white/5 space-y-3">
                    <h5 class="text-white font-bold text-sm">ApplyUnii UK</h5>
                    <p class="text-gray-500 text-xs leading-relaxed">
                        Preston, United Kingdom<br />
                        Ribble Saw Mill Paley Road Preston PR1 8LT
                    </p>
                    <p class="text-[#00d084] font-bold text-xs">+44 7733897140</p>
                </div>
            </div>

            <!-- Office Nepal -->
            <div>
                <!-- Extra top margin only on mobile if needed, otherwise matches UK -->
                <h4 class="text-white font-bold uppercase tracking-widest text-[10px] mb-8 lg:opacity-0">Our Offices</h4>
                <div class="p-6 rounded-2xl bg-[#0f172a]/50 border border-white/5 space-y-3">
                    <h5 class="text-white font-bold text-sm">ApplyUnii Nepal</h5>
                    <p class="text-gray-500 text-xs leading-relaxed">
                        Kathmandu, Nepal<br />
                        Kathmandu Nepal
                    </p>
                    <p class="text-[#00d084] font-bold text-xs">+977 9811943139</p>
                </div>
            </div>
        </div>

        <!-- Bottom Bar -->
        <div class="pt-8 border-t border-white/5 flex flex-col md:flex-row justify-between items-center gap-6">
            <p class="text-gray-500 text-[10px]">© 2026 ApplyUnii. All rights reserved.</p>
            <div class="flex gap-8">
                <a href="/" class="text-gray-500 hover:text-white text-[10px] transition-colors">Privacy Policy</a>
                <a href="/" class="text-gray-500 hover:text-white text-[10px] transition-colors">Terms of Service</a>
            </div>
        </div>
    </div>
</footer>