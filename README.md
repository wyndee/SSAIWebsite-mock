<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Skyguard Security Agency Inc.</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        .custom-input {
            background-color: #f1f5f9; 
            color: #1e293b;
            border: 1px solid #cbd5e1;
            border-radius: 0.75rem;
            padding: 0.75rem 1rem;
            width: 100%;
            outline: none;
            transition: border-color 0.2s;
        }
        .custom-input:focus {
            border-color: #f5a623;
        }
        .custom-select {
            appearance: none;
            background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' fill='none' viewBox='0 0 24 24' stroke='%2364748b'%3E%3Cpath stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='M19 9l-7 7-7-7'%3E%3C/path%3E%3C/svg%3E");
            background-repeat: no-repeat;
            background-position: right 1rem center;
            background-size: 1.2em 1.2em;
        }
        
        /* Modal Animation */
        .modal-enter { animation: fadeIn 0.3s ease-out forwards; }
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }
        
        /* Glowing Button Animation */
        @keyframes pulse-glow {
            0% { box-shadow: 0 0 5px rgba(245, 166, 35, 0.4); }
            50% { box-shadow: 0 0 20px rgba(245, 166, 35, 0.9); }
            100% { box-shadow: 0 0 5px rgba(245, 166, 35, 0.4); }
        }
        .glow-btn { animation: pulse-glow 2.5s infinite; }

        /* Scroll Reveal Animation */
        .reveal {
            opacity: 0;
            transform: translateY(40px);
            transition: all 0.8s ease-out;
        }
        .reveal.active {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body class="font-sans antialiased text-gray-800 bg-gray-50">

    <header class="bg-[#0a2342]/90 backdrop-blur-md w-full px-6 py-4 flex flex-col md:flex-row justify-between items-center z-[100] fixed top-0 border-b border-white/10 shadow-lg transition-all duration-300">
        <div class="flex items-center gap-4 mb-4 md:mb-0">
            <img src="Skyguard Eagle Head.png" alt="Skyguard Eagle" class="h-14 md:h-16 object-contain hover:scale-105 transition duration-300">
            <h1 class="text-white font-serif text-xl md:text-2xl font-bold tracking-wide">SKYGUARD SECURITY AGENCY INC.</h1>
        </div>
        <div>
            <a href="mailto:ssai.skyguard@gmail.com" class="text-white font-serif text-sm md:text-lg font-bold hover:text-[#f5a623] transition duration-300">SSAI.SKYGUARD@GMAIL.COM</a>
        </div>
    </header>

    <section class="relative min-h-screen flex items-center justify-center py-12 pt-24 overflow-hidden">
        <div class="absolute inset-0 z-0">
            <img src="Skyguard - Mock Website.png" alt="Skyguard Background" class="w-full h-full object-cover">
            <div class="absolute inset-0 bg-[#0a2342]/80"></div> 
        </div>

        <div class="relative z-10 container mx-auto px-6 grid md:grid-cols-2 gap-12 items-center reveal active">
            
            <div class="flex flex-col items-center md:items-start text-center md:text-left">
                <img src="Skyguard Logo.png" alt="Skyguard Logo" class="w-56 h-56 object-contain mb-8 drop-shadow-2xl hover:scale-105 transition duration-500">
                
                <h2 class="text-white font-serif text-4xl md:text-5xl font-bold uppercase leading-tight mb-4">
                    Soaring High Towards Excellence in Security and Safety Protection.
                </h2>
                <p class="text-gray-200 text-lg md:text-xl max-w-lg">
                    Premier elite protection and safety solutions across CALABARZON and NCR since 2021.
                </p>
            </div>

            <div class="bg-white rounded-[2rem] p-8 md:p-10 shadow-2xl w-full max-w-lg mx-auto transform transition-all duration-300 hover:-translate-y-2 hover:shadow-[0_20px_40px_rgba(0,0,0,0.4)]">
                <h3 class="text-[#0a2342] font-serif text-2xl font-bold text-center mb-2">HOW CAN WE HELP YOU?</h3>
                <p class="text-gray-500 text-sm text-center mb-6">
                    Your safety is a personal commitment to us. Tell us what you need and we'll build a shield of protection around it.
                </p>

                <form action="PASTE_YOUR_FORMSPREE_LINK_HERE" method="POST" class="space-y-4">
                    <input type="text" name="Full_Name" placeholder="Full Name / Company Name" class="custom-input" required>
                    <input type="email" name="Email_Address" placeholder="Email Address" class="custom-input" required>
                    <input type="tel" name="Contact_Number" placeholder="Contact Number" class="custom-input" required>
                    
                    <select name="Location" class="custom-input custom-select" required>
                        <option value="" disabled selected hidden>Location (NCR or CALABARZON)</option>
                        <optgroup label="NCR - Metro Manila">
                            <option value="Caloocan">Caloocan</option>
                            <option value="Las Piñas">Las Piñas</option>
                            <option value="Makati">Makati</option>
                            <option value="Malabon">Malabon</option>
                            <option value="Mandaluyong">Mandaluyong</option>
                            <option value="Manila">Manila</option>
                            <option value="Marikina">Marikina</option>
                            <option value="Muntinlupa">Muntinlupa</option>
                            <option value="Navotas">Navotas</option>
                            <option value="Parañaque">Parañaque</option>
                            <option value="Pasay">Pasay</option>
                            <option value="Pasig">Pasig</option>
                            <option value="Pateros">Pateros</option>
                            <option value="Quezon City">Quezon City</option>
                            <option value="San Juan">San Juan</option>
                            <option value="Taguig">Taguig</option>
                            <option value="Valenzuela">Valenzuela</option>
                        </optgroup>
                        <optgroup label="CALABARZON">
                            <option value="Antipolo">Antipolo</option>
                            <option value="Bacoor">Bacoor</option>
                            <option value="Batangas City">Batangas City</option>
                            <option value="Biñan">Biñan</option>
                            <option value="Cabuyao">Cabuyao</option>
                            <option value="Calamba">Calamba</option>
                            <option value="Cavite City">Cavite City</option>
                            <option value="Dasmariñas">Dasmariñas</option>
                            <option value="General Trias">General Trias</option>
                            <option value="Imus">Imus</option>
                            <option value="Lipa">Lipa</option>
                            <option value="Lucena">Lucena</option>
                            <option value="San Pablo">San Pablo</option>
                            <option value="San Pedro">San Pedro</option>
                            <option value="Santa Rosa">Santa Rosa</option>
                            <option value="Tagaytay">Tagaytay</option>
                            <option value="Tanauan">Tanauan</option>
                            <option value="Tayabas">Tayabas</option>
                            <option value="Trece Martires">Trece Martires</option>
                        </optgroup>
                    </select>

                    <select name="Service_Needed" class="custom-input custom-select" required>
                        <option value="" disabled selected hidden>Type of Service Needed</option>
                        <option value="Residential">Residential Community Security</option>
                        <option value="Commercial">Commercial / Retail Security</option>
                        <option value="Industrial">Industrial Plant Protection</option>
                        <option value="Tourism">Theme Park & Tourism Security</option>
                        <option value="Healthcare">Healthcare & Medical Facilities</option>
                        <option value="Academic">Academic Institution Safety</option>
                    </select>

                    <textarea name="Message" placeholder="Brief Message / Security Requirements" rows="3" class="custom-input resize-none" required></textarea>

                    <button type="submit" class="w-full bg-[#f5a623] hover:bg-[#d48c1c] text-white font-bold text-lg py-3 rounded-xl transition duration-300 shadow-md glow-btn">
                        Get a Free Quote
                    </button>
                </form>
            </div>
        </div>
    </section>

    <section class="bg-gray-100 py-20 px-6">
        <div class="container mx-auto max-w-6xl reveal">
            <div class="grid md:grid-cols-2 gap-12">
                <div class="transition-all duration-300 hover:-translate-y-1">
                    <h2 class="text-[#0a2342] font-serif text-3xl md:text-4xl font-bold mb-6">Company Background</h2>
                    <p class="text-gray-700 leading-relaxed mb-8">
                        Skyguard Security Agency Inc. is the brainchild of a team of highly competitive and dedicated professionals. Leveraging years of experience in managing top-tier security agencies, we envisioned a company that doesn't just provide security services, but imparts expertise. We are aligned with our clients' goals to deliver not just safety, but total peace of mind.
                    </p>
                    
                    <h3 class="text-xl font-bold text-[#0a2342] mb-4 border-b-2 border-[#f5a623] inline-block pb-1">Strategic Headquarters</h3>
                    <ul class="space-y-4 text-sm text-gray-700 mt-4">
                        <li class="flex items-start gap-3 p-2 rounded-lg hover:bg-white hover:shadow-sm transition group">
                            <span class="text-[#f5a623] text-lg mt-1 group-hover:scale-125 transition-transform duration-300">📍</span>
                            <div>
                                <strong class="block text-[#0a2342]">Current HQ (Approved Dec 29, 2023):</strong>
                                <a href="https://www.google.com/maps/place/Skyguard+Security+Agency+Inc./@14.2779636,121.1060639,21z/data=!4m6!3m5!1s0x3397d90070e7024f:0x2446d074338b48ee!8m2!3d14.2778764!4d121.1061124!16s%2Fg%2F11w3l060qg?entry=ttu&g_ep=EgoyMDI2MDMwNS4wIKXMDSoASAFQAw%3D%3D" target="_blank" class="hover:text-[#f5a623] hover:underline transition duration-300 block mt-1">
                                    Block 3, Lot 6, Phase 1-C Annex, San Lorenzo South, Brgy. Dita, Santa Rosa City, Laguna.
                                </a>
                            </div>
                        </li>

                        <li class="flex items-start gap-3 mt-4 pt-4 border-t border-gray-200">
                            <span class="text-[#f5a623] text-lg mt-1">🗺️</span>
                            <div>
                                <strong class="block text-[#0a2342]">Operational Coverage:</strong>
                                CALABARZON & NCR Regions
                            </div>
                        </li>
                    </ul>
                </div>

                <div class="bg-white p-8 rounded-2xl shadow-lg border-t-4 border-[#0a2342] h-fit transition-all duration-500 hover:-translate-y-2 hover:shadow-2xl">
                    <h3 class="text-2xl font-bold text-[#0a2342] mb-6">Full Accreditation & Legal Compliance</h3>
                    <ul class="space-y-6 text-gray-700">
                        <li class="flex gap-4 items-start group">
                            <span class="bg-[#f5a623] text-white rounded-full p-1 mt-1 group-hover:scale-110 transition">
                                <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path></svg>
                            </span>
                            <span class="leading-relaxed">Duly registered with the <strong>Philippine National Police - SOSIA</strong>, and fully aligned with all government requisites.</span>
                        </li>
                        <li class="flex gap-4 items-start group">
                            <span class="bg-[#f5a623] text-white rounded-full p-1 mt-1 group-hover:scale-110 transition">
                                <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path></svg>
                            </span>
                            <span class="leading-relaxed">Operating in accordance with the provisions of <strong>Republic Act No. 11917</strong> (The Private Security Services Industry Act).</span>
                        </li>
                        <li class="flex gap-4 items-start group">
                            <span class="bg-[#f5a623] text-white rounded-full p-1 mt-1 group-hover:scale-110 transition">
                                <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path></svg>
                            </span>
                            <span class="leading-relaxed">Strictly compliant with <strong>DOLE standards (DO 174)</strong>.</span>
                        </li>
                        <li class="flex gap-4 items-start group">
                            <span class="bg-[#f5a623] text-white rounded-full p-1 mt-1 group-hover:scale-110 transition">
                                <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path></svg>
                            </span>
                            <span class="leading-relaxed">Proud Member of <strong>PADPAO Region IV</strong>.</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <section class="py-20 px-6 container mx-auto reveal">
        <div class="grid md:grid-cols-2 gap-8 max-w-5xl mx-auto">
            <div class="bg-white p-8 rounded-2xl shadow-lg border-t-4 border-[#0a2342] transition-all duration-300 hover:-translate-y-2 hover:shadow-2xl">
                <h3 class="text-2xl font-bold text-[#0a2342] mb-4">Our Mission</h3>
                <p class="text-gray-600 leading-relaxed">At SKYGUARD, we take pride in providing superior, extraordinaire security, safety services and protection with integrity to all our clients and customers for total satisfaction and peace of mind.</p>
            </div>
            <div class="bg-white p-8 rounded-2xl shadow-lg border-t-4 border-[#f5a623] transition-all duration-300 hover:-translate-y-2 hover:shadow-2xl">
                <h3 class="text-2xl font-bold text-[#f5a623] mb-4">Our Vision</h3>
                <p class="text-gray-600 leading-relaxed">To be at par with the top security agencies in the country, providing quality services through continuous investment in equipment and well-trained personnel that is committed to excellence to ensure the security and protection of every client’s life and property.</p>
            </div>
        </div>
    </section>

    <section class="py-16 px-6 bg-white border-t border-gray-100 reveal">
        <div class="container mx-auto max-w-5xl">
            <h2 class="text-[#0a2342] font-serif text-3xl md:text-4xl font-bold text-center mb-12">Our Culture</h2>
            <div class="flex flex-col gap-y-4 max-w-2xl mx-auto">
                <div class="flex items-center gap-6 p-4 rounded-xl bg-gray-50 border border-gray-100 shadow-sm hover:shadow-lg hover:-translate-y-1 hover:border-[#f5a623]/30 transition-all duration-300 cursor-default">
                    <span class="text-5xl font-bold text-[#f5a623] font-serif w-12 text-center drop-shadow-sm">S</span>
                    <p class="text-gray-700 font-medium text-lg">uperior Security and Safety Services</p>
                </div>
                <div class="flex items-center gap-6 p-4 rounded-xl bg-gray-50 border border-gray-100 shadow-sm hover:shadow-lg hover:-translate-y-1 hover:border-[#f5a623]/30 transition-all duration-300 cursor-default">
                    <span class="text-5xl font-bold text-[#f5a623] font-serif w-12 text-center drop-shadow-sm">K</span>
                    <p class="text-gray-700 font-medium text-lg">nowledgeable and Well-Trained Personnel and Administration</p>
                </div>
                <div class="flex items-center gap-6 p-4 rounded-xl bg-gray-50 border border-gray-100 shadow-sm hover:shadow-lg hover:-translate-y-1 hover:border-[#f5a623]/30 transition-all duration-300 cursor-default">
                    <span class="text-5xl font-bold text-[#f5a623] font-serif w-12 text-center drop-shadow-sm">Y</span>
                    <p class="text-gray-700 font-medium text-lg">earning for Continuous Improvement and Growth</p>
                </div>
                <div class="flex items-center gap-6 p-4 rounded-xl bg-gray-50 border border-gray-100 shadow-sm hover:shadow-lg hover:-translate-y-1 hover:border-[#f5a623]/30 transition-all duration-300 cursor-default">
                    <span class="text-5xl font-bold text-[#f5a623] font-serif w-12 text-center drop-shadow-sm">G</span>
                    <p class="text-gray-700 font-medium text-lg">eared towards Excellence</p>
                </div>
                <div class="flex items-center gap-6 p-4 rounded-xl bg-gray-50 border border-gray-100 shadow-sm hover:shadow-lg hover:-translate-y-1 hover:border-[#f5a623]/30 transition-all duration-300 cursor-default">
                    <span class="text-5xl font-bold text-[#f5a623] font-serif w-12 text-center drop-shadow-sm">U</span>
                    <p class="text-gray-700 font-medium text-lg">pdated on the latest in Security Industry Regulation</p>
                </div>
                <div class="flex items-center gap-6 p-4 rounded-xl bg-gray-50 border border-gray-100 shadow-sm hover:shadow-lg hover:-translate-y-1 hover:border-[#f5a623]/30 transition-all duration-300 cursor-default">
                    <span class="text-5xl font-bold text-[#f5a623] font-serif w-12 text-center drop-shadow-sm">A</span>
                    <p class="text-gray-700 font-medium text-lg">daptive to any Work Environment</p>
                </div>
                <div class="flex items-center gap-6 p-4 rounded-xl bg-gray-50 border border-gray-100 shadow-sm hover:shadow-lg hover:-translate-y-1 hover:border-[#f5a623]/30 transition-all duration-300 cursor-default">
                    <span class="text-5xl font-bold text-[#f5a623] font-serif w-12 text-center drop-shadow-sm">R</span>
                    <p class="text-gray-700 font-medium text-lg">esult-Driven</p>
                </div>
                <div class="flex items-center gap-6 p-4 rounded-xl bg-gray-50 border border-gray-100 shadow-sm hover:shadow-lg hover:-translate-y-1 hover:border-[#f5a623]/30 transition-all duration-300 cursor-default">
                    <span class="text-5xl font-bold text-[#f5a623] font-serif w-12 text-center drop-shadow-sm">D</span>
                    <p class="text-gray-700 font-medium text-lg">uty-bound to provide the highest level of client satisfaction</p>
                </div>
            </div>
        </div>
    </section>

    <section class="bg-[#0a2342] py-20 px-6 reveal">
        <div class="container mx-auto text-center">
            <h2 class="text-white font-serif text-3xl md:text-4xl font-bold mb-12">Our Core Values: The APIRR Standard</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 lg:grid-cols-5 gap-6 max-w-6xl mx-auto">
                <div class="bg-white/10 p-6 rounded-xl border border-white/20 backdrop-blur-sm transition-all duration-300 hover:-translate-y-2 hover:bg-white/20">
                    <h4 class="text-[#f5a623] text-xl font-bold mb-3">Accountability</h4>
                    <p class="text-sm text-gray-200">We take full ownership of our actions, honoring commitments and standing behind every decision.</p>
                </div>
                <div class="bg-white/10 p-6 rounded-xl border border-white/20 backdrop-blur-sm transition-all duration-300 hover:-translate-y-2 hover:bg-white/20">
                    <h4 class="text-[#f5a623] text-xl font-bold mb-3">Proactivity</h4>
                    <p class="text-sm text-gray-200">We don't just react; we anticipate. We neutralize threats before they become problems.</p>
                </div>
                <div class="bg-white/10 p-6 rounded-xl border border-white/20 backdrop-blur-sm transition-all duration-300 hover:-translate-y-2 hover:bg-white/20">
                    <h4 class="text-[#f5a623] text-xl font-bold mb-3">Integrity</h4>
                    <p class="text-sm text-gray-200">Honesty is our non-negotiable foundation, operating with strict ethical standards.</p>
                </div>
                <div class="bg-white/10 p-6 rounded-xl border border-white/20 backdrop-blur-sm transition-all duration-300 hover:-translate-y-2 hover:bg-white/20">
                    <h4 class="text-[#f5a623] text-xl font-bold mb-3">Reliability</h4>
                    <p class="text-sm text-gray-200">Trustworthy and consistent. Rain or shine, Skyguard is always present and ready.</p>
                </div>
                <div class="bg-white/10 p-6 rounded-xl border border-white/20 backdrop-blur-sm transition-all duration-300 hover:-translate-y-2 hover:bg-white/20">
                    <h4 class="text-[#f5a623] text-xl font-bold mb-3">Resiliency</h4>
                    <p class="text-sm text-gray-200">Built to withstand pressure. We adapt, overcome, and remain steadfast in high-stakes environments.</p>
                </div>
            </div>
        </div>
    </section>

    <section class="py-20 px-6 bg-gray-100 reveal">
        <div class="container mx-auto max-w-6xl">
            <h2 class="text-[#0a2342] font-serif text-3xl md:text-4xl font-bold text-center mb-12">Gallery & Operations</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                
                <div onclick="openModal('modal-rcsu')" class="cursor-pointer group rounded-2xl overflow-hidden shadow-lg bg-white border border-gray-200 relative transition-all duration-500 hover:-translate-y-2 hover:shadow-2xl">
                    <div class="h-64 w-full bg-[#0a2342] flex items-center justify-center relative overflow-hidden">
                        <img src="photos/rcsu-inspection.jpg" alt="RCSU Inspection" class="w-full h-full object-cover group-hover:scale-110 transition duration-700">
                        <div class="absolute inset-0 bg-black/40 flex items-center justify-center opacity-0 group-hover:opacity-100 transition duration-300">
                            <span class="text-white font-bold tracking-wider uppercase border-2 border-white px-4 py-2 rounded-lg">View Album</span>
                        </div>
                    </div>
                    <div class="p-4 bg-[#0a2342] border-t-4 border-[#f5a623]">
                        <h4 class="text-white font-bold text-center text-lg group-hover:text-[#f5a623] transition duration-300">RCSU Inspection</h4>
                    </div>
                </div>

                <div onclick="openModal('modal-training')" class="cursor-pointer group rounded-2xl overflow-hidden shadow-lg bg-white border border-gray-200 relative transition-all duration-500 hover:-translate-y-2 hover:shadow-2xl">
                    <div class="h-64 w-full bg-[#0a2342] flex items-center justify-center relative overflow-hidden">
                        <img src="photos/training-seminar.jpg" alt="Training and Seminar" class="w-full h-full object-cover group-hover:scale-110 transition duration-700">
                        <div class="absolute inset-0 bg-black/40 flex items-center justify-center opacity-0 group-hover:opacity-100 transition duration-300">
                            <span class="text-white font-bold tracking-wider uppercase border-2 border-white px-4 py-2 rounded-lg">View Album</span>
                        </div>
                    </div>
                    <div class="p-4 bg-[#0a2342] border-t-4 border-[#f5a623]">
                        <h4 class="text-white font-bold text-center text-lg group-hover:text-[#f5a623] transition duration-300">Training & Seminars</h4>
                    </div>
                </div>

                <div onclick="openModal('modal-action')" class="cursor-pointer group rounded-2xl overflow-hidden shadow-lg bg-white border border-gray-200 relative transition-all duration-500 hover:-translate-y-2 hover:shadow-2xl">
                    <div class="h-64 w-full bg-[#0a2342] flex items-center justify-center relative overflow-hidden">
                        <img src="photos/skyguard-action.jpg" alt="Skyguard in Action" class="w-full h-full object-cover group-hover:scale-110 transition duration-700">
                        <div class="absolute inset-0 bg-black/40 flex items-center justify-center opacity-0 group-hover:opacity-100 transition duration-300">
                            <span class="text-white font-bold tracking-wider uppercase border-2 border-white px-4 py-2 rounded-lg">View Album</span>
                        </div>
                    </div>
                    <div class="p-4 bg-[#0a2342] border-t-4 border-[#f5a623]">
                        <h4 class="text-white font-bold text-center text-lg group-hover:text-[#f5a623] transition duration-300">Skyguard in Action</h4>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <footer class="bg-[#0a2342] border-t-4 border-[#f5a623] pt-16 pb-8 px-6 mt-12 reveal">
        <div class="container mx-auto max-w-6xl">
            <div class="grid md:grid-cols-2 gap-12 items-center mb-12 border-b border-white/10 pb-12">
                
                <div class="text-center md:text-left">
                    <h2 class="text-white font-serif text-3xl font-bold mb-4">Ready for Total Peace of Mind?</h2>
                    <p class="text-gray-300 mb-6 text-lg">Let us build a shield of protection around what matters most to you. Partner with the elite today.</p>
                    <a href="#" onclick="window.scrollTo({top: 0, behavior: 'smooth'}); return false;" class="inline-block bg-transparent border-2 border-[#f5a623] text-[#f5a623] hover:bg-[#f5a623] hover:text-white font-bold py-3 px-8 rounded-xl transition duration-300">
                        Get Your Free Quote
                    </a>
                </div>

                <div class="bg-white/5 p-8 rounded-2xl border border-white/10 text-center md:text-left backdrop-blur-sm transition-all duration-300 hover:bg-white/10 hover:-translate-y-1 shadow-2xl">
                    <h2 class="text-white font-serif text-2xl font-bold mb-3 flex items-center justify-center md:justify-start gap-3">
                        <span class="text-[#f5a623]">🛡️</span> Join the Skyguard Fleet
                    </h2>
                    <p class="text-gray-300 text-sm mb-6 leading-relaxed">
                        We are actively looking for highly trained, disciplined, and licensed security professionals to join our growing team. Please have your <strong>LESP ID</strong> ready for verification.
                    </p>
                    <a href="PASTE_YOUR_GOOGLE_FORM_LINK_HERE" target="_blank" class="inline-block w-full text-center bg-[#f5a623] hover:bg-[#d48c1c] text-white font-bold text-lg py-3 px-6 rounded-xl transition duration-300 shadow-lg glow-btn">
                        Apply Now
                    </a>
                </div>

            </div>

            <div class="text-center text-gray-400 text-sm flex flex-col md:flex-row justify-between items-center opacity-70">
                <p>© 2026 Skyguard Security Agency Inc. All rights reserved.</p>
                <p class="mt-2 md:mt-0">Soaring High Towards Excellence.</p>
            </div>
        </div>
    </footer>

    <div id="modal-rcsu" class="hidden fixed inset-0 z-[100] bg-black/95 overflow-y-auto modal-enter p-4 md:p-10">
        <div class="flex justify-between items-center mb-8">
            <h3 class="text-white text-2xl md:text-3xl font-bold font-serif">RCSU Inspection Album</h3>
            <button onclick="closeModal('modal-rcsu')" class="text-white hover:text-[#f5a623] text-4xl font-bold transition transform hover:scale-110">×</button>
        </div>
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 max-w-7xl mx-auto">
            <img src="photos/rcsu-1.jpg" alt="RCSU Photo" class="w-full h-64 md:h-80 object-cover rounded-xl shadow-lg border border-gray-700 hover:border-[#f5a623] transition">
            <img src="photos/rcsu-2.jpg" alt="RCSU Photo" class="w-full h-64 md:h-80 object-cover rounded-xl shadow-lg border border-gray-700 hover:border-[#f5a623] transition">
            <img src="photos/rcsu-3.jpg" alt="RCSU Photo" class="w-full h-64 md:h-80 object-cover rounded-xl shadow-lg border border-gray-700 hover:border-[#f5a623] transition">
        </div>
    </div>

    <div id="modal-training" class="hidden fixed inset-0 z-[100] bg-black/95 overflow-y-auto modal-enter p-4 md:p-10">
        <div class="flex justify-between items-center mb-8">
            <h3 class="text-white text-2xl md:text-3xl font-bold font-serif">Training & Seminars Album</h3>
            <button onclick="closeModal('modal-training')" class="text-white hover:text-[#f5a623] text-4xl font-bold transition transform hover:scale-110">×</button>
        </div>
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 max-w-7xl mx-auto">
            <img src="photos/training-1.jpg" alt="Training Photo" class="w-full h-64 md:h-80 object-cover rounded-xl shadow-lg border border-gray-700 hover:border-[#f5a623] transition">
            <img src="photos/training-2.jpg" alt="Training Photo" class="w-full h-64 md:h-80 object-cover rounded-xl shadow-lg border border-gray-700 hover:border-[#f5a623] transition">
            <img src="photos/training-3.jpg" alt="Training Photo" class="w-full h-64 md:h-80 object-cover rounded-xl shadow-lg border border-gray-700 hover:border-[#f5a623] transition">
        </div>
    </div>

    <div id="modal-action" class="hidden fixed inset-0 z-[100] bg-black/95 overflow-y-auto modal-enter p-4 md:p-10">
        <div class="flex justify-between items-center mb-8">
            <h3 class="text-white text-2xl md:text-3xl font-bold font-serif">Skyguard in Action Album</h3>
            <button onclick="closeModal('modal-action')" class="text-white hover:text-[#f5a623] text-4xl font-bold transition transform hover:scale-110">×</button>
        </div>
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 max-w-7xl mx-auto">
            <img src="photos/action-1.jpg" alt="Action Photo" class="w-full h-64 md:h-80 object-cover rounded-xl shadow-lg border border-gray-700 hover:border-[#f5a623] transition">
            <img src="photos/action-2.jpg" alt="Action Photo" class="w-full h-64 md:h-80 object-cover rounded-xl shadow-lg border border-gray-700 hover:border-[#f5a623] transition">
            <img src="photos/action-3.jpg" alt="Action Photo" class="w-full h-64 md:h-80 object-cover rounded-xl shadow-lg border border-gray-700 hover:border-[#f5a623] transition">
        </div>
    </div>

    <script>
        function openModal(modalId) {
            document.getElementById(modalId).classList.remove('hidden');
            document.body.style.overflow = 'hidden'; 
        }
        function closeModal(modalId) {
            document.getElementById(modalId).classList.add('hidden');
            document.body.style.overflow = 'auto'; 
        }

        document.addEventListener("DOMContentLoaded", function() {
            const reveals = document.querySelectorAll(".reveal");
            const observer = new IntersectionObserver((entries) => {
                entries.forEach((entry) => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add("active");
                    }
                });
            }, { threshold: 0.1 });
            
            reveals.forEach((reveal) => {
                observer.observe(reveal);
            });
        });
    </script>

</body>
</html>
