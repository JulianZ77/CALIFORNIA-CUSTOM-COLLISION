# CALIFORNIA-CUSTOM-COLLISION
We specialize in repairing cars that have been in collisions
<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>California Custom Collision - Santa Clarita's Elite Auto Body Repair</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            dark: '#0f172a', /* slate-900 */
                            card: '#1e293b', /* slate-800 */
                            gold: '#fbbf24', /* amber-400 */
                            goldHover: '#f59e0b', /* amber-500 */
                            accent: '#38bdf8', /* sky-400 */
                        }
                    }
                }
            }
        }
    </script>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght=300;400;500;600;700;800&family=Space+Grotesk:wght=500;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: #0b0f19;
        }
        h1, h2, h3, .font-display {
            font-family: 'Space Grotesk', sans-serif;
        }
        /* Hide scrollbar for clean custom UI experience */
        .no-scrollbar::-webkit-scrollbar {
            display: none;
        }
        .no-scrollbar {
            -ms-overflow-style: none;
            scrollbar-width: none;
        }
    </style>
</head>
<body class="text-slate-100 selection:bg-amber-400 selection:text-slate-900">

    <!-- HEADER / NAVIGATION -->
    <header class="sticky top-0 z-50 bg-slate-950/85 backdrop-blur-md border-b border-slate-800/80 transition-all duration-300">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            <!-- Logo -->
            <a href="#" class="flex items-center space-x-3 group">
                <div class="bg-gradient-to-tr from-amber-500 to-amber-300 p-2.5 rounded-xl shadow-lg shadow-amber-500/10 group-hover:scale-105 transition-transform">
                    <svg class="w-6 h-6 text-slate-950" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M13 10V3L4 14h7v7l9-11h-7z" />
                    </svg>
                </div>
                <div>
                    <span class="text-lg font-bold tracking-tight block text-white font-display">CALIFORNIA CUSTOM</span>
                    <span class="text-xs tracking-widest text-amber-400 block font-semibold uppercase -mt-1">Collision Repair</span>
                </div>
            </a>

            <!-- Desktop Nav -->
            <nav class="hidden md:flex items-center space-x-8 text-sm font-medium text-slate-300">
                <a href="#estimator" class="hover:text-amber-400 transition-colors">Cost Estimator</a>
                <a href="#services" class="hover:text-amber-400 transition-colors">Services</a>
                <a href="#before-after" class="hover:text-amber-400 transition-colors">Our Work</a>
                <a href="#insurance" class="hover:text-amber-400 transition-colors">Insurance</a>
                <a href="#about" class="hover:text-amber-400 transition-colors">Why Us</a>
            </nav>

            <!-- CTA Buttons -->
            <div class="hidden md:flex items-center space-x-4">
                <a href="tel:+16616663242" class="text-sm font-semibold text-slate-300 hover:text-white flex items-center gap-2 transition-colors">
                    <svg class="w-4 h-4 text-amber-400" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M2.25 6.75c0 8.284 6.716 15 15 15h2.25a2.25 2.25 0 002.25-2.25v-1.372c0-.516-.351-.966-.852-1.091l-4.423-1.106c-.44-.11-.902.055-1.173.417l-.97 1.293c-.282.376-.769.542-1.21.387a12.035 12.035 0 01-7.108-7.108c-.155-.44.01-1.29-.387l1.293-.97a1.125 1.125 0 00.417-1.173L6.963 3.102a1.125 1.125 0 00-1.091-.852H4.5A2.25 2.25 0 002.25 4.5v2.25z"/></svg>
                    (661) 666-3242
                </a>
                <a href="#book-appointment" class="bg-gradient-to-r from-amber-500 to-amber-400 text-slate-950 font-semibold px-5 py-2.5 rounded-xl shadow-lg shadow-amber-500/10 hover:shadow-amber-500/20 hover:scale-[1.02] transition-all text-sm">
                    Book Inspection
                </a>
            </div>

            <!-- Mobile Menu Button -->
            <button id="mobile-menu-btn" class="md:hidden p-2 text-slate-400 hover:text-white focus:outline-none" aria-label="Toggle Menu">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path id="menu-icon-open" class="block" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"/>
                    <path id="menu-icon-close" class="hidden" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"/>
                </svg>
            </button>
        </div>

        <!-- Mobile Nav Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-slate-950/95 border-b border-slate-800 px-4 pt-2 pb-6 space-y-3">
            <a href="#estimator" class="block py-2.5 px-3 rounded-lg hover:bg-slate-900 text-slate-300 hover:text-amber-400 font-medium transition-all" onclick="toggleMobileMenu()">Cost Estimator</a>
            <a href="#services" class="block py-2.5 px-3 rounded-lg hover:bg-slate-900 text-slate-300 hover:text-amber-400 font-medium transition-all" onclick="toggleMobileMenu()">Services</a>
            <a href="#before-after" class="block py-2.5 px-3 rounded-lg hover:bg-slate-900 text-slate-300 hover:text-amber-400 font-medium transition-all" onclick="toggleMobileMenu()">Our Work</a>
            <a href="#insurance" class="block py-2.5 px-3 rounded-lg hover:bg-slate-900 text-slate-300 hover:text-amber-400 font-medium transition-all" onclick="toggleMobileMenu()">Insurance Helpers</a>
            <a href="#about" class="block py-2.5 px-3 rounded-lg hover:bg-slate-900 text-slate-300 hover:text-amber-400 font-medium transition-all" onclick="toggleMobileMenu()">Why Us</a>
            <hr class="border-slate-800 my-2">
            <div class="pt-2 flex flex-col gap-3 px-3">
                <a href="tel:+16616663242" class="text-sm font-semibold text-slate-300 hover:text-white flex items-center gap-2">
                    <svg class="w-4 h-4 text-amber-400" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M2.25 6.75c0 8.284 6.716 15 15 15h2.25a2.25 2.25 0 002.25-2.25v-1.372c0-.516-.351-.966-.852-1.091l-4.423-1.106c-.44-.11-.902.055-1.173.417l-.97 1.293c-.282.376-.769.542-1.21.387a12.035 12.035 0 01-7.108-7.108c-.155-.44.01-1.29-.387l1.293-.97a1.125 1.125 0 00.417-1.173L6.963 3.102a1.125 1.125 0 00-1.091-.852H4.5A2.25 2.25 0 002.25 4.5v2.25z"/></svg>
                    (661) 666-3242
                </a>
                <a href="#book-appointment" onclick="toggleMobileMenu()" class="text-center bg-gradient-to-r from-amber-500 to-amber-400 text-slate-950 font-bold py-3 rounded-xl shadow-lg transition-all">
                    Book Free Inspection
                </a>
            </div>
        </div>
    </header>

    <!-- HERO SECTION -->
    <section class="relative overflow-hidden pt-12 pb-20 md:py-32 bg-slate-950">
        <!-- Background Grid Pattern -->
        <div class="absolute inset-0 bg-[linear-gradient(to_right,#0f172a_1px,transparent_1px),linear-gradient(to_bottom,#0f172a_1px,transparent_1px)] bg-[size:4rem_4rem] [mask-image:radial-gradient(ellipse_60%_50%_at_50%_0%,#000_70%,transparent_100%)] opacity-60"></div>
        
        <!-- Amber Glows -->
        <div class="absolute top-0 left-1/4 w-96 h-96 bg-amber-500/10 rounded-full blur-[120px] pointer-events-none"></div>
        <div class="absolute bottom-12 right-1/4 w-96 h-96 bg-sky-500/10 rounded-full blur-[120px] pointer-events-none"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                
                <!-- Left Text Content -->
                <div class="lg:col-span-7 text-center lg:text-left space-y-6">
                    <!-- Badge -->
                    <span class="inline-flex items-center gap-1.5 px-3 py-1 rounded-full text-xs font-bold bg-amber-400/10 text-amber-400 border border-amber-400/20 uppercase tracking-widest mx-auto lg:mx-0">
                        <span class="w-1.5 h-1.5 rounded-full bg-amber-400 animate-pulse"></span>
                        Premium Structural &amp; Auto Paint Finishers
                    </span>

                    <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold tracking-tight text-white leading-[1.1] font-display">
                        Flawless Repairs for <br class="hidden sm:inline">
                        <span class="bg-gradient-to-r from-amber-400 via-yellow-300 to-sky-400 bg-clip-text text-transparent">California Custom Collision</span>
                    </h1>

                    <p class="text-base sm:text-lg text-slate-300 max-w-xl mx-auto lg:mx-0 leading-relaxed">
                        Accidents happen, but the damage doesn’t have to last. From high-grade Tesla structural alignments to precision paint color matching in Newhall and Santa Clarita, we restore your luxury or daily vehicle back to OEM factory specifications.
                    </p>

                    <!-- Trust Stats Grid -->
                    <div class="grid grid-cols-3 gap-4 py-3 border-y border-slate-800/80 max-w-md mx-auto lg:mx-0">
                        <div class="text-center lg:text-left">
                            <span class="block text-2xl sm:text-3xl font-bold font-display text-white">4.9★</span>
                            <span class="text-xs text-slate-400 font-medium">Top Rated Santa Clarita Shop</span>
                        </div>
                        <div class="text-center lg:text-left border-x border-slate-800 px-2">
                            <span class="block text-2xl sm:text-3xl font-bold font-display text-white">I-CAR</span>
                            <span class="text-xs text-slate-400 font-medium">Gold Class certified</span>
                        </div>
                        <div class="text-center lg:text-left">
                            <span class="block text-2xl sm:text-3xl font-bold font-display text-white">Lifetime</span>
                            <span class="text-xs text-slate-400 font-medium">Repair warranty</span>
                        </div>
                    </div>

                    <!-- Actions -->
                    <div class="flex flex-col sm:flex-row gap-4 justify-center lg:justify-start pt-2">
                        <a href="#estimator" class="bg-gradient-to-r from-amber-500 to-amber-400 text-slate-950 font-bold px-8 py-4 rounded-xl shadow-xl shadow-amber-500/10 hover:shadow-amber-500/25 hover:scale-[1.02] active:scale-[0.98] transition-all flex items-center justify-center gap-2">
                            <span>Calculate Cost Instantly</span>
                            <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M17.25 8.25L21 12m0 0l-3.75 3.75M21 12H3"/></svg>
                        </a>
                        <a href="#book-appointment" class="bg-slate-900 hover:bg-slate-800 border border-slate-800 text-white font-semibold px-8 py-4 rounded-xl hover:scale-[1.02] active:scale-[0.98] transition-all flex items-center justify-center gap-2">
                            <span>Schedule Inspection</span>
                        </a>
                    </div>
                </div>

                <!-- Right Hero Visual Block -->
                <div class="lg:col-span-5 relative">
                    <div class="relative mx-auto max-w-md lg:max-w-none bg-slate-900 border border-slate-800/80 rounded-3xl p-6 overflow-hidden shadow-2xl shadow-black/80">
                        <div class="absolute -top-12 -right-12 w-40 h-40 bg-amber-500/20 rounded-full blur-3xl"></div>
                        
                        <div class="flex items-center justify-between mb-4 pb-4 border-b border-slate-800">
                            <div class="flex items-center gap-2">
                                <span class="w-3 h-3 rounded-full bg-red-500"></span>
                                <span class="w-3 h-3 rounded-full bg-yellow-500"></span>
                                <span class="w-3 h-3 rounded-full bg-green-500"></span>
                            </div>
                            <span class="text-xs font-semibold text-slate-400 tracking-wider uppercase">Live Shop Queue</span>
                        </div>

                        <!-- Progress Queue Items -->
                        <div class="space-y-4">
                            <div class="bg-slate-950/70 p-3.5 rounded-xl border border-slate-800 flex items-center justify-between">
                                <div class="flex items-center gap-3">
                                    <div class="w-10 h-10 rounded-lg bg-amber-500/10 border border-amber-500/30 flex items-center justify-center font-bold text-amber-400 font-display">T</div>
                                    <div>
                                        <h4 class="text-sm font-semibold text-white">Tesla Model S</h4>
                                        <p class="text-xs text-slate-400">Quarter panel PDR &amp; Align</p>
                                    </div>
                                </div>
                                <span class="px-2.5 py-1 rounded-full text-[10px] font-bold bg-amber-500/10 text-amber-400 uppercase tracking-wider">In Paint Booth</span>
                            </div>

                            <div class="bg-slate-950/70 p-3.5 rounded-xl border border-slate-800 flex items-center justify-between">
                                <div class="flex items-center gap-3">
                                    <div class="w-10 h-10 rounded-lg bg-sky-500/10 border border-sky-500/30 flex items-center justify-center font-bold text-sky-400 font-display">F</div>
                                    <div>
                                        <h4 class="text-sm font-semibold text-white">Ford F-150 Lightning</h4>
                                        <p class="text-xs text-slate-400">Rear structural bedside repair</p>
                                    </div>
                                </div>
                                <span class="px-2.5 py-1 rounded-full text-[10px] font-bold bg-sky-500/10 text-sky-400 uppercase tracking-wider">Frame Aligned</span>
                            </div>

                            <div class="bg-slate-950/70 p-3.5 rounded-xl border border-slate-800 flex items-center justify-between">
                                <div class="flex items-center gap-3">
                                    <div class="w-10 h-10 rounded-lg bg-emerald-500/10 border border-emerald-500/30 flex items-center justify-center font-bold text-emerald-400 font-display">P</div>
                                    <div>
                                        <h4 class="text-sm font-semibold text-white">Porsche Taycan</h4>
                                        <p class="text-xs text-slate-400">Bumper micro-paint correction</p>
                                    </div>
                                </div>
                                <span class="px-2.5 py-1 rounded-full text-[10px] font-bold bg-emerald-500/10 text-emerald-400 uppercase tracking-wider">Ready / Detailing</span>
                            </div>
                        </div>

                        <!-- Local Quick Contact Footer -->
                        <div class="mt-6 pt-4 border-t border-slate-800 text-center">
                            <p class="text-xs text-slate-400">🚗 Locally operated at 22432 12th St, Newhall</p>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- INTERACTIVE BEFORE/AFTER SLIDER SECTION -->
    <section id="before-after" class="py-20 bg-slate-900/60 border-t border-b border-slate-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-12">
                <span class="text-xs font-bold text-amber-400 tracking-widest uppercase block mb-2">Our Standards Speak for Themselves</span>
                <h2 class="text-3xl sm:text-4xl font-bold text-white font-display">Slide to See our Repair Magic</h2>
                <p class="text-slate-400 mt-3 text-sm sm:text-base">
                    Drag the slider to compare the initial collision damage against our post-repair precision color match finish. No shortcuts, just perfection.
                </p>
            </div>

            <div class="max-w-4xl mx-auto relative select-none">
                <!-- Wrapper Box for Before/After Images -->
                <div class="relative aspect-[16/9] w-full rounded-2xl overflow-hidden shadow-2xl border border-slate-800 bg-slate-950">
                    
                    <!-- AFTER IMAGE CONTAINER (Full background, the restored luxury sedan) -->
                    <div class="absolute inset-0 w-full h-full bg-slate-900 flex items-center justify-center">
                        <div class="relative w-full h-full flex items-center justify-center p-4">
                            <div class="absolute inset-0 opacity-10 bg-[radial-gradient(#ffffff_1px,transparent_1px)] [background-size:16px_16px]"></div>
                            <!-- Perfect Car SVG -->
                            <svg class="w-[85%] h-auto text-slate-300 drop-shadow-[0_0_35px_rgba(56,189,248,0.15)]" viewBox="0 0 800 350" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <rect width="800" height="350" rx="16" fill="#0f172a" />
                                <path d="M120 230 C 130 190, 180 120, 300 110 C 350 110, 480 110, 540 130 C 620 150, 710 190, 720 230 C 725 250, 680 260, 600 260 C 580 260, 560 230, 510 230 C 460 230, 440 260, 360 260 C 280 260, 260 230, 210 230 C 160 230, 140 260, 120 260 C 100 260, 115 250, 120 230 Z" fill="#334155" />
                                <path d="M280 120 C 330 118, 480 118, 520 135 C 570 150, 640 180, 670 215 C 675 220, 600 220, 510 220 C 490 220, 470 210, 430 210 C 390 210, 370 220, 290 220 C 210 220, 190 210, 150 210 C 145 210, 200 160, 280 120 Z" fill="#475569" />
                                <path d="M300 125 L 420 125 L 420 170 L 320 170 Z" fill="#1e293b" stroke="#64748b" stroke-width="3"/>
                                <path d="M435 125 L 515 135 L 505 170 L 435 170 Z" fill="#1e293b" stroke="#64748b" stroke-width="3"/>
                                <circle cx="210" cy="245" r="45" fill="#0f172a" stroke="#fbbf24" stroke-width="6" />
                                <circle cx="210" cy="245" r="25" fill="#334155" stroke="#94a3b8" stroke-width="4" />
                                <circle cx="510" cy="245" r="45" fill="#0f172a" stroke="#fbbf24" stroke-width="6" />
                                <circle cx="510" cy="245" r="25" fill="#334155" stroke="#94a3b8" stroke-width="4" />
                                <path d="M120 210 L 140 215 L 135 230 Z" fill="#38bdf8" class="animate-pulse" />
                                <path d="M710 210 L 690 215 L 695 230 Z" fill="#ef4444" />
                                <path d="M300 135 Q 400 128 500 140" stroke="#ffffff" stroke-dasharray="10 5" stroke-width="3" stroke-linecap="round" opacity="0.4" />
                            </svg>
                            <div class="absolute bottom-6 right-6 bg-emerald-500/95 text-slate-950 font-bold px-4 py-1.5 rounded-full text-xs flex items-center gap-1.5 shadow-lg">
                                <span class="w-1.5 h-1.5 rounded-full bg-slate-950 animate-ping"></span>
                                RESTORED TO OEM SPECS
                            </div>
                        </div>
                    </div>

                    <!-- BEFORE IMAGE CONTAINER (Dynamically resized using JS width adjustment) -->
                    <div id="before-image-container" class="absolute inset-0 w-1/2 h-full bg-slate-950 overflow-hidden border-r-2 border-amber-400">
                        <div class="absolute inset-0 w-full h-full flex items-center justify-center p-4 bg-slate-950" style="width: 100%; min-width: 800px;">
                            <div class="absolute inset-0 opacity-5 bg-[radial-gradient(#ffffff_1px,transparent_1px)] [background-size:16px_16px]"></div>
                            <!-- Damaged Car SVG -->
                            <svg class="w-[85%] h-auto text-slate-500" viewBox="0 0 800 350" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <rect width="800" height="350" rx="16" fill="#090d16" />
                                <path d="M120 230 C 130 190, 180 120, 300 110 C 350 110, 480 110, 540 130 C 600 140, 640 180, 660 210 C 630 220, 610 200, 590 225 C 570 245, 590 260, 580 260 C 560 260, 560 230, 510 230 C 460 230, 440 260, 360 260 C 280 260, 260 230, 210 230 C 160 230, 140 260, 120 260 C 100 260, 115 250, 120 230 Z" fill="#1e293b" />
                                <path d="M280 120 C 330 118, 480 118, 520 135 C 540 142, 590 180, 600 210 C 565 210, 550 195, 530 215 C 510 220, 470 210, 430 210 C 390 210, 370 220, 290 220 C 210 220, 190 210, 150 210 C 145 210, 200 160, 280 120 Z" fill="#334155" />
                                <path d="M300 125 L 420 125 L 420 170 L 320 170 Z" fill="#0f172a" stroke="#475569" stroke-width="3"/>
                                <path d="M435 125 L 515 135 L 505 170 L 435 170 Z" fill="#0f172a" stroke="#475569" stroke-width="3"/>
                                <circle cx="210" cy="245" r="45" fill="#090d16" stroke="#475569" stroke-width="6" />
                                <circle cx="210" cy="245" r="25" fill="#1e293b" stroke="#334155" stroke-width="4" />
                                <path d="M465 255 Q 510 220 555 255 Z" stroke="#334155" stroke-width="6" fill="#090d16" />
                                <path d="M570 170 Q 590 190 560 220 M 580 180 Q 610 210 590 230" stroke="#ef4444" stroke-width="4" stroke-linecap="round" />
                                <path d="M605 200 L 650 180 M 610 210 L 640 200" stroke="#94a3b8" stroke-width="3" stroke-linecap="round" />
                                <path d="M660 210 L 640 215 L 645 225 Z" fill="#7f1d1d" />
                            </svg>
                            <div class="absolute bottom-6 left-6 bg-red-500/95 text-white font-bold px-4 py-1.5 rounded-full text-xs flex items-center gap-1.5 shadow-lg">
                                <span class="w-1.5 h-1.5 rounded-full bg-white animate-ping"></span>
                                COLLISION DAMAGE
                            </div>
                        </div>
                    </div>

                    <!-- SLIDER DRAG BAR -->
                    <div id="slider-handle" class="absolute top-0 bottom-0 left-1/2 w-1 -ml-0.5 bg-amber-400 cursor-ew-resize flex items-center justify-center z-30">
                        <div class="w-10 h-10 bg-slate-900 border-2 border-amber-400 text-amber-400 rounded-full flex items-center justify-center shadow-xl hover:scale-110 active:scale-95 transition-all">
                            <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 15L12 18.75 15.75 15m-7.5-6L12 5.25 15.75 9" transform="rotate(90 12 12)" />
                            </svg>
                        </div>
                    </div>
                </div>

                <div class="text-center mt-4">
                    <p class="text-xs text-slate-500 italic flex items-center justify-center gap-1">
                        <span>← Swipe or drag slider handle left/right to compare →</span>
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- INTERACTIVE ESTIMATOR & SCHEDULER SECTION -->
    <section id="estimator" class="py-20 bg-slate-950 relative">
        <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[600px] h-[600px] bg-amber-500/5 rounded-full blur-[140px] pointer-events-none"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-start">
                
                <!-- Left Details & Instructions -->
                <div class="lg:col-span-5 space-y-6">
                    <span class="text-xs font-bold text-amber-400 tracking-widest uppercase block">Transparent Pricing</span>
                    <h2 class="text-3xl sm:text-4xl font-bold text-white font-display">Instant Repair Cost Estimator</h2>
                    <p class="text-slate-300 leading-relaxed">
                        We believe auto collision repair shouldn't come with surprises. Select your vehicle area and severity level below to get an instant estimated benchmark range of what your collision or PDR repair would cost with California Custom Collision.
                    </p>
                    
                    <div class="space-y-4">
                        <div class="flex items-start gap-3">
                            <div class="w-8 h-8 rounded-full bg-amber-400/10 text-amber-400 flex items-center justify-center font-bold flex-shrink-0">1</div>
                            <p class="text-slate-300 text-sm">Select the damaged section of your vehicle on the right card.</p>
                        </div>
                        <div class="flex items-start gap-3">
                            <div class="w-8 h-8 rounded-full bg-amber-400/10 text-amber-400 flex items-center justify-center font-bold flex-shrink-0">2</div>
                            <p class="text-slate-300 text-sm">Pick the damage level—ranging from cosmetic scratches to heavier frame-distorting impacts.</p>
                        </div>
                        <div class="flex items-start gap-3">
                            <div class="w-8 h-8 rounded-full bg-amber-400/10 text-amber-400 flex items-center justify-center font-bold flex-shrink-0">3</div>
                            <p class="text-slate-300 text-sm">Review your instant pricing and schedule an in-person precision blueprinting session.</p>
                        </div>
                    </div>

                    <div class="bg-slate-900 border border-slate-800 p-5 rounded-2xl flex items-center gap-4">
                        <div class="p-3 bg-sky-500/10 text-sky-400 rounded-xl">
                            <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9 12.75L11.25 15 15 9.75m-3-7.036A11.959 11.959 0 013.598 6 11.99 11.99 0 003 9.749c0 5.592 3.824 10.29 9 11.623 5.176-1.332 9-6.03 9-11.622 0-1.31-.21-2.57-.598-3.751h-.152c-3.196 0-6.1-1.248-8.25-3.285z"/></svg>
                        </div>
                        <div>
                            <h4 class="text-sm font-semibold text-white">Insurance Claims Assistance</h4>
                            <p class="text-xs text-slate-400">Our specialists coordinate directly with all major insurance adjusters.</p>
                        </div>
                    </div>
                </div>

                <!-- Right Estimator Widget Interface -->
                <div class="lg:col-span-7 bg-slate-900 border border-slate-800 rounded-3xl p-6 sm:p-8 shadow-2xl">
                    <form id="estimator-form" class="space-y-6">
                        
                        <!-- Panel Selector Grid -->
                        <div>
                            <label class="block text-sm font-semibold text-slate-300 mb-3">1. Damage Location</label>
                            <div class="grid grid-cols-2 sm:grid-cols-3 gap-3">
                                <button type="button" onclick="selectEstimatorPanel('bumper-front', 350)" class="panel-btn border-2 border-slate-800 bg-slate-950 p-4 rounded-xl text-left hover:border-amber-400/60 transition-all flex flex-col justify-between h-24 focus:outline-none">
                                    <span class="text-xs text-slate-400 font-semibold tracking-wider uppercase">Front</span>
                                    <span class="text-sm font-bold text-white">Front Bumper</span>
                                </button>
                                <button type="button" onclick="selectEstimatorPanel('door-panel', 450)" class="panel-btn border-2 border-slate-800 bg-slate-950 p-4 rounded-xl text-left hover:border-amber-400/60 transition-all flex flex-col justify-between h-24 focus:outline-none">
                                    <span class="text-xs text-slate-400 font-semibold tracking-wider uppercase">Side</span>
                                    <span class="text-sm font-bold text-white">Door / Panel</span>
                                </button>
                                <button type="button" onclick="selectEstimatorPanel('fender-quarter', 500)" class="panel-btn border-2 border-slate-800 bg-slate-950 p-4 rounded-xl text-left hover:border-amber-400/60 transition-all flex flex-col justify-between h-24 focus:outline-none">
                                    <span class="text-xs text-slate-400 font-semibold tracking-wider uppercase">Corner</span>
                                    <span class="text-sm font-bold text-white">Fender / Quarter</span>
                                </button>
                                <button type="button" onclick="selectEstimatorPanel('hood-trunk', 600)" class="panel-btn border-2 border-slate-800 bg-slate-950 p-4 rounded-xl text-left hover:border-amber-400/60 transition-all flex flex-col justify-between h-24 focus:outline-none">
                                    <span class="text-xs text-slate-400 font-semibold tracking-wider uppercase">Top</span>
                                    <span class="text-sm font-bold text-white">Hood / Trunk</span>
                                </button>
                                <button type="button" onclick="selectEstimatorPanel('bumper-rear', 380)" class="panel-btn border-2 border-slate-800 bg-slate-950 p-4 rounded-xl text-left hover:border-amber-400/60 transition-all flex flex-col justify-between h-24 focus:outline-none">
                                    <span class="text-xs text-slate-400 font-semibold tracking-wider uppercase">Rear</span>
                                    <span class="text-sm font-bold text-white">Rear Bumper</span>
                                </button>
                                <button type="button" onclick="selectEstimatorPanel('windshield', 250)" class="panel-btn border-2 border-slate-800 bg-slate-950 p-4 rounded-xl text-left hover:border-amber-400/60 transition-all flex flex-col justify-between h-24 focus:outline-none">
                                    <span class="text-xs text-slate-400 font-semibold tracking-wider uppercase">Glass</span>
                                    <span class="text-sm font-bold text-white">Windshield</span>
                                </button>
                            </div>
                        </div>

                        <!-- Damage Severity Selector -->
                        <div>
                            <label class="block text-sm font-semibold text-slate-300 mb-3">2. Damage Severity</label>
                            <div class="grid grid-cols-1 sm:grid-cols-3 gap-3">
                                <button type="button" onclick="selectEstimatorSeverity('light', 1.0)" class="severity-btn border-2 border-slate-800 bg-slate-950 p-4 rounded-xl text-left hover:border-amber-400/60 transition-all focus:outline-none">
                                    <span class="block text-sm font-bold text-white">Light Scratch / Ding</span>
                                    <span class="block text-xs text-slate-400 mt-1">Primarily cosmetic paint correction or light PDR.</span>
                                </button>
                                <button type="button" onclick="selectEstimatorSeverity('moderate', 1.8)" class="severity-btn border-2 border-slate-800 bg-slate-950 p-4 rounded-xl text-left hover:border-amber-400/60 transition-all focus:outline-none">
                                    <span class="block text-sm font-bold text-white">Moderate Dent</span>
                                    <span class="block text-xs text-slate-400 mt-1">Deep creased dents requiring reshaping & refinishing.</span>
                                </button>
                                <button type="button" onclick="selectEstimatorSeverity('heavy', 3.5)" class="severity-btn border-2 border-slate-800 bg-slate-950 p-4 rounded-xl text-left hover:border-amber-400/60 transition-all focus:outline-none">
                                    <span class="block text-sm font-bold text-white">Heavy Collision</span>
                                    <span class="block text-xs text-slate-400 mt-1">Structural panel realignment, parts replacement & deep matching.</span>
                                </button>
                            </div>
                        </div>

                        <!-- Results Dashboard -->
                        <div class="bg-slate-950/80 border border-slate-800 rounded-2xl p-6 flex flex-col sm:flex-row items-center justify-between gap-6">
                            <div>
                                <span class="text-xs font-semibold text-slate-400 uppercase tracking-widest block">Estimated Repair Range</span>
                                <span id="estimate-output" class="text-3xl sm:text-4xl font-extrabold text-amber-400 font-display mt-1 block">Select choices...</span>
                                <span id="estimate-time" class="text-xs text-slate-400 mt-1.5 block">Select elements above to forecast turnaround.</span>
                            </div>
                            <a href="#book-appointment" class="w-full sm:w-auto text-center bg-gradient-to-r from-amber-500 to-amber-400 hover:from-amber-600 hover:to-amber-500 text-slate-950 font-bold px-6 py-3 rounded-xl shadow-lg transition-all text-sm whitespace-nowrap">
                                Lock In Quote Rate
                            </a>
                        </div>
                    </form>
                </div>

            </div>
        </div>
    </section>

    <!-- CORE SPECIALIZED SERVICES -->
    <section id="services" class="py-20 bg-slate-900/40 border-y border-slate-800/80 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <span class="text-xs font-bold text-amber-400 tracking-widest uppercase block mb-2">Our Specialized Body Shop</span>
                <h2 class="text-3xl sm:text-4xl font-bold text-white font-display">Craftsmanship Meets Modern Tech</h2>
                <p class="text-slate-400 mt-3 text-sm sm:text-base">
                    California Custom Collision combines high-end precision diagnostic scanning tools with veteran collision technicians to provide safe, beautiful, factory-grade auto restorations.
                </p>
            </div>

            <!-- Services Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                
                <!-- Service Card 1 -->
                <div class="bg-slate-900 border border-slate-800/80 p-6 rounded-2xl hover:border-slate-700 hover:translate-y-[-4px] transition-all duration-300 flex flex-col justify-between">
                    <div>
                        <div class="w-12 h-12 bg-amber-400/10 text-amber-400 rounded-xl flex items-center justify-center mb-5">
                            <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9.53 16.122l9.37-9.37m0 0a3 3 0 114.243 4.242l-9.37 9.379m-9.37-9.379a3 3 0 014.243-4.242l9.37 9.378m-9.37-9.378l1.524 1.524m-9.001 8.83l1.852-1.851m-1.852 1.851a1.5 1.5 0 01-2.122-2.122l1.851-1.852m0 0l1.37 1.37"/></svg>
                        </div>
                        <h3 class="text-lg font-bold text-white mb-2 font-display">Precision Color Matching</h3>
                        <p class="text-slate-400 text-sm leading-relaxed">
                            Using computerized spectro-photometer paint color scanning, we perfectly match the age, fade, and tone of your existing factory coat, leaving zero seam lines.
                        </p>
                    </div>
                    <a href="#book-appointment" class="text-amber-400 hover:text-amber-300 text-xs font-bold tracking-wider uppercase mt-6 inline-flex items-center gap-1.5 transition-colors">
                        Free Inspection
                        <span>→</span>
                    </a>
                </div>

                <!-- Service Card 2 -->
                <div class="bg-slate-900 border border-slate-800/80 p-6 rounded-2xl hover:border-slate-700 hover:translate-y-[-4px] transition-all duration-300 flex flex-col justify-between">
                    <div>
                        <div class="w-12 h-12 bg-amber-400/10 text-amber-400 rounded-xl flex items-center justify-center mb-5">
                            <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M12 9v6m3-3H9m12 0a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
                        </div>
                        <h3 class="text-lg font-bold text-white mb-2 font-display">Computerized Frame Alignment</h3>
                        <p class="text-slate-400 text-sm leading-relaxed">
                            Heavy impacts can displace critical frame elements. Our specialized structural alignment benches restore your frame back to within 1mm of exact safety specs.
                        </p>
                    </div>
                    <a href="#book-appointment" class="text-amber-400 hover:text-amber-300 text-xs font-bold tracking-wider uppercase mt-6 inline-flex items-center gap-1.5 transition-colors">
                        Free Inspection
                        <span>→</span>
                    </a>
                </div>

                <!-- Service Card 3 -->
                <div class="bg-slate-900 border border-slate-800/80 p-6 rounded-2xl hover:border-slate-700 hover:translate-y-[-4px] transition-all duration-300 flex flex-col justify-between">
                    <div>
                        <div class="w-12 h-12 bg-amber-400/10 text-amber-400 rounded-xl flex items-center justify-center mb-5">
                            <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M19.5 12c0-1.232-.046-2.453-.138-3.662a4.006 4.006 0 00-3.7-3.7 48.678 48.678 0 00-7.324 0 4.006 4.006 0 00-3.7 3.7c-.017.22-.032.441-.046.662M19.5 12l3-3m-3 3l-3-3m-12 3c0 1.232.046 2.453.138 3.662a4.006 4.006 0 003.7 3.7 48.656 48.656 0 007.324 0 4.006 4.006 0 003.7-3.7c.017-.22.032-.441.046-.662M4.5 12l3 3m-3-3l-3 3"/></svg>
                        </div>
                        <h3 class="text-lg font-bold text-white mb-2 font-display">Paintless Dent Repair (PDR)</h3>
                        <p class="text-slate-400 text-sm leading-relaxed">
                            For minor door dings and Santa Clarita valley hail storms. Our technicians sculpt metal from behind the panel, preserving your precious factory paint completely.
                        </p>
                    </div>
                    <a href="#book-appointment" class="text-amber-400 hover:text-amber-300 text-xs font-bold tracking-wider uppercase mt-6 inline-flex items-center gap-1.5 transition-colors">
                        Free Inspection
                        <span>→</span>
                    </a>
                </div>

                <!-- Service Card 4 -->
                <div class="bg-slate-900 border border-slate-800/80 p-6 rounded-2xl hover:border-slate-700 hover:translate-y-[-4px] transition-all duration-300 flex flex-col justify-between">
                    <div>
                        <div class="w-12 h-12 bg-amber-400/10 text-amber-400 rounded-xl flex items-center justify-center mb-5">
                            <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M11.42 15.17L17.25 21A2.67 2.67 0 1021 17.25l-5.83-5.83m-4.32 4.32a9.044 9.044 0 0112.53-12.53m-12.53 12.53l-4.76-4.76M9.96 11.47l-4.32 4.32M2.25 21l3-3M21 2.25l-3 3"/></svg>
                        </div>
                        <h3 class="text-lg font-bold text-white mb-2 font-display">ADAS Sensor Calibration</h3>
                        <p class="text-slate-400 text-sm leading-relaxed">
                            Modern cars rely on radar and camera sensors inside bumpers and mirrors. We perform safety re-calibration to make sure your driver-assist lanes and braking work safely.
                        </p>
                    </div>
                    <a href="#book-appointment" class="text-amber-400 hover:text-amber-300 text-xs font-bold tracking-wider uppercase mt-6 inline-flex items-center gap-1.5 transition-colors">
                        Free Inspection
                        <span>→</span>
                    </a>
                </div>

                <!-- Service Card 5 -->
                <div class="bg-slate-900 border border-slate-800/80 p-6 rounded-2xl hover:border-slate-700 hover:translate-y-[-4px] transition-all duration-300 flex flex-col justify-between">
                    <div>
                        <div class="w-12 h-12 bg-amber-400/10 text-amber-400 rounded-xl flex items-center justify-center mb-5">
                            <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M11.25 4.5l7.5 7.5-7.5 7.5m-6-15l7.5 7.5-7.5 7.5"/></svg>
                        </div>
                        <h3 class="text-lg font-bold text-white mb-2 font-display">Glass &amp; Windshield Restoration</h3>
                        <p class="text-slate-400 text-sm leading-relaxed">
                            From minor freeway star-burst chips on the I-5 or SR-14 to shattered structural windshield side glass, we handle fast, flawless, safety-rated glass replacement.
                        </p>
                    </div>
                    <a href="#book-appointment" class="text-amber-400 hover:text-amber-300 text-xs font-bold tracking-wider uppercase mt-6 inline-flex items-center gap-1.5 transition-colors">
                        Free Inspection
                        <span>→</span>
                    </a>
                </div>

                <!-- Service Card 6 -->
                <div class="bg-slate-900 border border-slate-800/80 p-6 rounded-2xl hover:border-slate-700 hover:translate-y-[-4px] transition-all duration-300 flex flex-col justify-between">
                    <div>
                        <div class="w-12 h-12 bg-amber-400/10 text-amber-400 rounded-xl flex items-center justify-center mb-5">
                            <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z"/></svg>
                        </div>
                        <h3 class="text-lg font-bold text-white mb-2 font-display">Lifetime Limited Warranty</h3>
                        <p class="text-slate-400 text-sm leading-relaxed">
                            Our confidence is backed by a written lifetime limited warranty on all panel works, metal shaping, structure alignment, and luxury paint coats.
                        </p>
                    </div>
                    <a href="#book-appointment" class="text-amber-400 hover:text-amber-300 text-xs font-bold tracking-wider uppercase mt-6 inline-flex items-center gap-1.5 transition-colors">
                        View Details
                        <span>→</span>
                    </a>
                </div>

            </div>
        </div>
    </section>

    <!-- INTERACTIVE INSURANCE COORDINATION HELPER -->
    <section id="insurance" class="py-20 bg-slate-950">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <span class="text-xs font-bold text-amber-400 tracking-widest uppercase block mb-2">Stress-Free Claims Process</span>
                <h2 class="text-3xl sm:text-4xl font-bold text-white font-display">Seamless Claim Coordination</h2>
                <p class="text-slate-400 mt-3 text-sm sm:text-base">
                    Filing a claim can be stressful. We coordinate directly with every single major insurance provider, managing paperwork and scheduling adjusters to minimize your out-of-pocket costs.
                </p>
            </div>

            <!-- Interactive Provider Selection -->
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                
                <!-- Provider Logo Selector -->
                <div class="lg:col-span-5 grid grid-cols-2 gap-4">
                    <button type="button" onclick="selectInsuranceProvider('aaa')" class="insurance-logo-btn bg-slate-900 border border-slate-800 p-6 rounded-2xl flex items-center justify-center hover:border-amber-400/40 hover:scale-105 transition-all text-xl font-extrabold text-slate-300">
                        AAA Insurance
                    </button>
                    <button type="button" onclick="selectInsuranceProvider('geico')" class="insurance-logo-btn bg-slate-900 border border-slate-800 p-6 rounded-2xl flex items-center justify-center hover:border-amber-400/40 hover:scale-105 transition-all text-xl font-extrabold text-slate-300">
                        GEICO
                    </button>
                    <button type="button" onclick="selectInsuranceProvider('statefarm')" class="insurance-logo-btn bg-slate-900 border border-slate-800 p-6 rounded-2xl flex items-center justify-center hover:border-amber-400/40 hover:scale-105 transition-all text-xl font-extrabold text-slate-300">
                        State Farm
                    </button>
                    <button type="button" onclick="selectInsuranceProvider('progressive')" class="insurance-logo-btn bg-slate-900 border border-slate-800 p-6 rounded-2xl flex items-center justify-center hover:border-amber-400/40 hover:scale-105 transition-all text-xl font-extrabold text-slate-300">
                        Progressive
                    </button>
                </div>

                <!-- Custom Claim Instruction Output Card -->
                <div class="lg:col-span-7 bg-slate-900 border border-slate-800/80 rounded-3xl p-8 shadow-xl">
                    <div id="insurance-detail-content" class="space-y-6">
                        <!-- Default prompt shown before clicking -->
                        <div class="text-center py-8">
                            <span class="inline-flex p-3 rounded-full bg-amber-400/10 text-amber-400 mb-4">
                                <svg class="w-8 h-8" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M11.25 11.25l.041-.02a.75.75 0 11.517 1.361l-.04.02-1.12.56a.75.75 0 00-.417.672v1.02a.75.75 0 01-1.5 0v-1.02a2.25 2.25 0 011.25-2.014l1.12-.56zm.25-2.25a.75.75 0 110-1.5.75.75 0 010 1.5z"/><path stroke-linecap="round" stroke-linejoin="round" d="M18.364 18.364A9 9 0 005.636 5.636m12.728 12.728A9 9 0 015.636 5.636m12.728 12.728L5.636 5.636"/></svg>
                            </span>
                            <h3 class="text-xl font-bold text-white font-display">Select an Insurance Provider</h3>
                            <p class="text-sm text-slate-400 mt-2 max-w-sm mx-auto">
                                Click any provider logo on the left to see our customized direct-billing agreement guidelines &amp; how we streamline your out-of-pocket costs.
                            </p>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- TESTIMONIALS & PROOF -->
    <section class="py-20 bg-slate-900/60 border-t border-b border-slate-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row md:items-end justify-between mb-16">
                <div>
                    <span class="text-xs font-bold text-amber-400 tracking-widest uppercase block mb-2">Real Local Reviews</span>
                    <h2 class="text-3xl sm:text-4xl font-bold text-white font-display">Loved by Santa Clarita Drivers</h2>
                </div>
                <p class="text-slate-400 mt-3 md:mt-0 text-sm max-w-md">
                    From Old Town Newhall to Valencia commuters, see why SCV local drivers highly rate our speed, honesty, and seamless custom color blending.
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                
                <!-- Testimonial 1 -->
                <div class="bg-slate-900 border border-slate-800 p-6 rounded-2xl flex flex-col justify-between">
                    <div>
                        <div class="flex items-center gap-1 text-amber-400 mb-4">
                            <svg class="w-5 h-5 fill-current" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                            <svg class="w-5 h-5 fill-current" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                            <svg class="w-5 h-5 fill-current" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                            <svg class="w-5 h-5 fill-current" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                            <svg class="w-5 h-5 fill-current" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                        </div>
                        <p class="text-slate-300 text-sm leading-relaxed italic">
                            "Someone swiped my brand new Model Y bumper in a parking lot. California Custom Collision made the insurance claim trivial. When I picked it up, the finish was absolutely identical to the factory paint. Zero lines!"
                        </p>
                    </div>
                    <div class="mt-6 pt-4 border-t border-slate-800 flex items-center justify-between">
                        <div>
                            <span class="block text-sm font-bold text-white">David K.</span>
                            <span class="block text-xs text-slate-400">Valencia, CA</span>
                        </div>
                        <span class="text-xs font-semibold bg-emerald-500/10 text-emerald-400 px-2 py-1 rounded-full uppercase tracking-wider">Tesla Owner</span>
                    </div>
                </div>

                <!-- Testimonial 2 -->
                <div class="bg-slate-900 border border-slate-800 p-6 rounded-2xl flex flex-col justify-between">
                    <div>
                        <div class="flex items-center gap-1 text-amber-400 mb-4">
                            <svg class="w-5 h-5 fill-current" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                            <svg class="w-5 h-5 fill-current" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                            <svg class="w-5 h-5 fill-current" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                            <svg class="w-5 h-5 fill-current" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                            <svg class="w-5 h-5 fill-current" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                        </div>
                        <p class="text-slate-300 text-sm leading-relaxed italic">
                            "A tree limb fell on my truck bedside during high winds. California Custom Collision handled the heavy duty frame restoration and replacement panels perfectly. Turnaround was extremely fast."
                        </p>
                    </div>
                    <div class="mt-6 pt-4 border-t border-slate-800 flex items-center justify-between">
                        <div>
                            <span class="block text-sm font-bold text-white">Robert M.</span>
                            <span class="block text-xs text-slate-400">Castaic, CA</span>
                        </div>
                        <span class="text-xs font-semibold bg-sky-500/10 text-sky-400 px-2 py-1 rounded-full uppercase tracking-wider">Ram Truck</span>
                    </div>
                </div>

                <!-- Testimonial 3 -->
                <div class="bg-slate-900 border border-slate-800 p-6 rounded-2xl flex flex-col justify-between">
                    <div>
                        <div class="flex items-center gap-1 text-amber-400 mb-4">
                            <svg class="w-5 h-5 fill-current" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                            <svg class="w-5 h-5 fill-current" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                            <svg class="w-5 h-5 fill-current" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                            <svg class="w-5 h-5 fill-current" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                            <svg class="w-5 h-5 fill-current" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                        </div>
                        <p class="text-slate-300 text-sm leading-relaxed italic">
                            "I had a deep parking lot dent on my Lexus door panel. They recommended Paintless Dent Repair (PDR). It took under an hour and looks totally flawless. Great local Newhall business."
                        </p>
                    </div>
                    <div class="mt-6 pt-4 border-t border-slate-800 flex items-center justify-between">
                        <div>
                            <span class="block text-sm font-bold text-white">Sarah T.</span>
                            <span class="block text-xs text-slate-400">Canyon Country, CA</span>
                        </div>
                        <span class="text-xs font-semibold bg-emerald-500/10 text-emerald-400 px-2 py-1 rounded-full uppercase tracking-wider">PDR Repair</span>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- DETAILED BOOKING APPOINTMENT & CONTACT FORM -->
    <section id="book-appointment" class="py-20 bg-slate-950 relative">
        <div class="absolute top-0 right-1/4 w-96 h-96 bg-amber-500/5 rounded-full blur-[120px] pointer-events-none"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-stretch">
                
                <!-- Left Details / Contact Info Cards -->
                <div class="lg:col-span-5 flex flex-col justify-between space-y-8">
                    <div>
                        <span class="text-xs font-bold text-amber-400 tracking-widest uppercase block mb-2">Ready to Book?</span>
                        <h2 class="text-3xl sm:text-4xl font-bold text-white font-display">Schedule Your Free Inspection Blueprinting</h2>
                        <p class="text-slate-400 mt-3 text-sm sm:text-base">
                            Bring your vehicle to our Newhall workshop, or have us inspect it while coordinating towing. We provide structured estimate printouts you can present directly to insurance adjusters.
                        </p>
                    </div>

                    <!-- Physical Contact Info Block -->
                    <div class="space-y-6">
                        <!-- Address -->
                        <div class="flex items-start gap-4">
                            <div class="p-3 bg-slate-900 border border-slate-800 text-amber-400 rounded-xl flex-shrink-0">
                                <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 11-6 0 3 3 0 016 0z"/><path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25s-7.5-4.108-7.5-11.25a7.5 7.5 0 1115 0z"/></svg>
                            </div>
                            <div>
                                <h4 class="text-sm font-bold text-white">California Custom Collision Workshop</h4>
                                <p class="text-xs text-slate-400 mt-0.5">22432 12th St, Santa Clarita, CA 91321</p>
                                <span class="text-[10px] text-slate-500 font-semibold block mt-1">(Near Old Town Newhall / Railroad Ave intersection)</span>
                            </div>
                        </div>

                        <!-- Phone / Contact -->
                        <div class="flex items-start gap-4">
                            <div class="p-3 bg-slate-900 border border-slate-800 text-amber-400 rounded-xl flex-shrink-0">
                                <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M2.25 6.75c0 8.284 6.716 15 15 15h2.25a2.25 2.25 0 002.25-2.25v-1.372c0-.516-.351-.966-.852-1.091l-4.423-1.106c-.44-.11-.902.055-1.173.417l-.97 1.293c-.282.376-.769.542-1.21.387a12.035 12.035 0 01-7.108-7.108c-.155-.44.01-1.29-.387l1.293-.97a1.125 1.125 0 00.417-1.173L6.963 3.102a1.125 1.125 0 00-1.091-.852H4.5A2.25 2.25 0 002.25 4.5v2.25z"/></svg>
                            </div>
                            <div>
                                <h4 class="text-sm font-bold text-white">Call Workshop</h4>
                                <p class="text-xs text-slate-400 mt-0.5">(661) 666-3242</p>
                                <span class="text-[10px] text-emerald-400 font-semibold block mt-1">● Live Support Available</span>
                            </div>
                        </div>

                        <!-- Operating Hours -->
                        <div class="flex items-start gap-4">
                            <div class="p-3 bg-slate-900 border border-slate-800 text-amber-400 rounded-xl flex-shrink-0">
                                <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M12 6v6h4.5m4.5 0a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
                            </div>
                            <div>
                                <h4 class="text-sm font-bold text-white">Hours of Operation</h4>
                                <p class="text-xs text-slate-400 mt-0.5">Monday – Friday: 7:30 AM – 6:00 PM</p>
                                <p class="text-xs text-slate-400">Saturday: 8:00 AM – 1:00 PM (By Appt)</p>
                            </div>
                        </div>
                    </div>

                    <!-- Custom Styled Map Representation -->
                    <div class="bg-slate-900 border border-slate-800 p-4 rounded-2xl relative overflow-hidden aspect-[4/2] flex items-center justify-center">
                        <div class="absolute inset-0 opacity-20 bg-[radial-gradient(#ffffff_1px,transparent_1px)] [background-size:20px_20px]"></div>
                        <svg class="absolute inset-0 w-full h-full text-slate-800" stroke="currentColor" stroke-width="2">
                            <line x1="10%" y1="0%" x2="90%" y2="100%" />
                            <line x1="0%" y1="50%" x2="100%" y2="50%" />
                            <line x1="30%" y1="100%" x2="30%" y2="0%" />
                        </svg>
                        <div class="relative z-10 text-center">
                            <span class="inline-flex p-2 bg-amber-400 text-slate-950 rounded-full mb-1 animate-bounce">
                                <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 11-6 0 3 3 0 016 0z"/><path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25s-7.5-4.108-7.5-11.25a7.5 7.5 0 1115 0z"/></svg>
                            </span>
                            <span class="block text-xs font-bold text-white uppercase tracking-wider">12th Street Shop</span>
                            <span class="block text-[10px] text-slate-400 mt-0.5">Downtown Newhall Area</span>
                        </div>
                    </div>
                </div>

                <!-- Right Form Box -->
                <div class="lg:col-span-7 bg-slate-900 border border-slate-800/80 rounded-3xl p-6 sm:p-8 shadow-xl flex flex-col justify-between">
                    <div>
                        <h3 class="text-xl font-bold text-white mb-6 font-display pb-3 border-b border-slate-800">Quick Appt Reservation</h3>
                        
                        <form id="appointment-form" onsubmit="handleFormSubmission(event)" class="space-y-4">
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-xs font-bold text-slate-400 uppercase tracking-wider mb-1">Full Name</label>
                                    <input type="text" required class="w-full bg-slate-950 border border-slate-800 focus:border-amber-400 focus:outline-none rounded-xl px-4 py-3 text-sm text-slate-200" placeholder="John Doe">
                                </div>
                                <div>
                                    <label class="block text-xs font-bold text-slate-400 uppercase tracking-wider mb-1">Phone Number</label>
                                    <input type="tel" required class="w-full bg-slate-950 border border-slate-800 focus:border-amber-400 focus:outline-none rounded-xl px-4 py-3 text-sm text-slate-200" placeholder="(661) 666-3242">
                                </div>
                            </div>

                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-xs font-bold text-slate-400 uppercase tracking-wider mb-1">Email Address</label>
                                    <input type="email" required class="w-full bg-slate-950 border border-slate-800 focus:border-amber-400 focus:outline-none rounded-xl px-4 py-3 text-sm text-slate-200" placeholder="john@example.com">
                                </div>
                                <div>
                                    <label class="block text-xs font-bold text-slate-400 uppercase tracking-wider mb-1">Vehicle Make/Model/Year</label>
                                    <input type="text" required class="w-full bg-slate-950 border border-slate-800 focus:border-amber-400 focus:outline-none rounded-xl px-4 py-3 text-sm text-slate-200" placeholder="e.g. 2024 Tesla Model Y">
                                </div>
                            </div>

                            <div>
                                <label class="block text-xs font-bold text-slate-400 uppercase tracking-wider mb-1">Primary Repair Needed</label>
                                <select class="w-full bg-slate-950 border border-slate-800 focus:border-amber-400 focus:outline-none rounded-xl px-4 py-3 text-sm text-slate-200">
                                    <option>Collision Repair &amp; Color Match</option>
                                    <option>Paintless Dent Repair (PDR)</option>
                                    <option>Bumper Damage / Replacement</option>
                                    <option>Windshield / Glass Repair</option>
                                    <option>Sensor/ADAS Calibration</option>
                                    <option>Insurance Consultation / Frame Inspection</option>
                                </select>
                            </div>

                            <div>
                                <label class="block text-xs font-bold text-slate-400 uppercase tracking-wider mb-1">Brief Description of Damage</label>
                                <textarea class="w-full bg-slate-950 border border-slate-800 focus:border-amber-400 focus:outline-none rounded-xl px-4 py-3 text-sm text-slate-200 h-24 resize-none" placeholder="Let us know what happened..."></textarea>
                            </div>

                            <div class="flex items-start gap-2 pt-2">
                                <input type="checkbox" id="consent" required class="mt-1 accent-amber-400 rounded">
                                <label for="consent" class="text-xs text-slate-400">
                                    I authorize California Custom Collision to call/text regarding my quote estimate details.
                                </label>
                            </div>

                            <button type="submit" class="w-full bg-gradient-to-r from-amber-500 to-amber-400 hover:from-amber-600 hover:to-amber-500 text-slate-950 font-bold py-4 rounded-xl shadow-lg hover:shadow-xl transition-all font-display text-base">
                                Send Inspection Booking Request
                            </button>
                        </form>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- CORE FAQ SECTION -->
    <section class="py-20 bg-slate-900/40 border-t border-slate-800">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <span class="text-xs font-bold text-amber-400 tracking-widest uppercase block mb-2">Have Questions?</span>
                <h2 class="text-3xl font-bold text-white font-display">Common Collision Repair FAQs</h2>
            </div>

            <div class="space-y-4">
                <!-- FAQ item 1 -->
                <div class="bg-slate-900 border border-slate-800 rounded-2xl p-5 cursor-pointer" onclick="toggleFaq('faq-1')">
                    <div class="flex items-center justify-between">
                        <h4 class="text-sm sm:text-base font-bold text-white">Do I have the right to choose my own repair shop?</h4>
                        <span id="faq-1-icon" class="text-amber-400 transition-transform font-bold text-xl">+</span>
                    </div>
                    <div id="faq-1" class="hidden mt-3 text-sm text-slate-400 leading-relaxed">
                        Absolutely. Under California Insurance Code Section 758.5, you have the full legal right to select any collision shop of your choice. Your insurance provider cannot force you to use their "preferred" or "network" shop.
                    </div>
                </div>

                <!-- FAQ item 2 -->
                <div class="bg-slate-900 border border-slate-800 rounded-2xl p-5 cursor-pointer" onclick="toggleFaq('faq-2')">
                    <div class="flex items-center justify-between">
                        <h4 class="text-sm sm:text-base font-bold text-white">How long will my bumper paint matching take?</h4>
                        <span id="faq-2-icon" class="text-amber-400 transition-transform font-bold text-xl">+</span>
                    </div>
                    <div id="faq-2" class="hidden mt-3 text-sm text-slate-400 leading-relaxed">
                        Standard bumper repairs and custom computer color matching usually take 2 to 4 business days. This allows correct prep work, primer application, perfect bake curing in our climate-controlled spray booths, and safe reassembly.
                    </div>
                </div>

                <!-- FAQ item 3 -->
                <div class="bg-slate-900 border border-slate-800 rounded-2xl p-5 cursor-pointer" onclick="toggleFaq('faq-3')">
                    <div class="flex items-center justify-between">
                        <h4 class="text-sm sm:text-base font-bold text-white">Do you handle hybrid and electric vehicle (EV) safety specs?</h4>
                        <span id="faq-3-icon" class="text-amber-400 transition-transform font-bold text-xl">+</span>
                    </div>
                    <div id="faq-3" class="hidden mt-3 text-sm text-slate-400 leading-relaxed">
                        Yes. Our technicians hold advanced EV structural certifications. We completely isolate active high-voltage battery arrays before doing heavy baking cycle color coats or structural frame realignment.
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-slate-950 border-t border-slate-800/80 py-12 text-slate-400 text-sm">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8 mb-8">
                <!-- Col 1 -->
                <div class="space-y-4">
                    <div class="flex items-center space-x-3">
                        <div class="bg-amber-400 p-2 rounded-lg">
                            <svg class="w-5 h-5 text-slate-950" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M13 10V3L4 14h7v7l9-11h-7z" />
                            </svg>
                        </div>
                        <span class="text-lg font-bold tracking-tight text-white font-display">California Custom</span>
                    </div>
                    <p class="text-xs text-slate-400 leading-relaxed">
                        Santa Clarita's premium destination for auto body structural alignment, state-of-the-art paint matching, and flawless collision repairs.
                    </p>
                </div>

                <!-- Col 2 -->
                <div>
                    <h5 class="text-white font-bold mb-4 font-display uppercase tracking-wider text-xs">Quick Navigation</h5>
                    <ul class="space-y-2 text-xs">
                        <li><a href="#estimator" class="hover:text-amber-400 transition-colors">Instant Repair Estimator</a></li>
                        <li><a href="#services" class="hover:text-amber-400 transition-colors">Specialized Services</a></li>
                        <li><a href="#before-after" class="hover:text-amber-400 transition-colors">Interactive Work Slider</a></li>
                        <li><a href="#insurance" class="hover:text-amber-400 transition-colors">Insurance Information</a></li>
                    </ul>
                </div>

                <!-- Col 3 -->
                <div>
                    <h5 class="text-white font-bold mb-4 font-display uppercase tracking-wider text-xs">Service Areas</h5>
                    <ul class="space-y-2 text-xs">
                        <li> Newhall, CA</li>
                        <li> Valencia, CA</li>
                        <li> Saugus, CA</li>
                        <li> Canyon Country &amp; Castaic</li>
                    </ul>
                </div>

                <!-- Col 4 -->
                <div>
                    <h5 class="text-white font-bold mb-4 font-display uppercase tracking-wider text-xs">Accreditation</h5>
                    <div class="space-y-2 text-xs text-slate-300">
                        <p>🏆 ASE Certified Technicians</p>
                        <p>🛡️ I-CAR Gold Class Certified</p>
                        <p>📄 Fully Bonded &amp; Insured California Shop</p>
                    </div>
                </div>
            </div>

            <div class="border-t border-slate-800 pt-8 flex flex-col sm:flex-row items-center justify-between gap-4">
                <p class="text-xs text-slate-500">&copy; 2026 California Custom Collision. All rights reserved.</p>
                <div class="flex space-x-6 text-xs text-slate-500">
                    <a href="#" class="hover:text-slate-300">Privacy Policy</a>
                    <a href="#" class="hover:text-slate-300">Terms of Service</a>
                </div>
            </div>
        </div>
    </footer>

    <!-- SUCCESS MODAL POPUP FOR BOOKINGS -->
    <div id="booking-modal" class="fixed inset-0 z-50 flex items-center justify-center p-4 bg-slate-950/80 backdrop-blur-sm hidden">
        <div class="bg-slate-900 border border-amber-400/30 rounded-3xl p-6 sm:p-8 max-w-md w-full text-center shadow-2xl relative">
            <div class="w-16 h-16 bg-amber-400/10 text-amber-400 rounded-full flex items-center justify-center mx-auto mb-5">
                <svg class="w-8 h-8" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M4.5 12.75l6 6 9-13.5"/>
                </svg>
            </div>
            <h3 class="text-2xl font-bold text-white font-display mb-2">Appointment Scheduled!</h3>
            <p id="modal-desc" class="text-sm text-slate-300 mb-6 leading-relaxed">
                Thank you for choosing California Custom Collision. A vehicle blueprinting specialist will call you at (661) 666-3242 to confirm your inspection details.
            </p>
            <button onclick="closeBookingModal()" class="w-full bg-gradient-to-r from-amber-500 to-amber-400 text-slate-950 font-bold py-3.5 rounded-xl">
                Awesome, Got It!
            </button>
        </div>
    </div>

    <!-- CORE LOGIC / SCRIPTS -->
    <script>
        // --- MOBILE MENU ---
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        const menuIconOpen = document.getElementById('menu-icon-open');
        const menuIconClose = document.getElementById('menu-icon-close');

        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
            menuIconOpen.classList.toggle('hidden');
            menuIconClose.classList.toggle('hidden');
        });

        function toggleMobileMenu() {
            mobileMenu.classList.add('hidden');
            menuIconOpen.classList.remove('hidden');
            menuIconClose.classList.add('hidden');
        }

        // --- BEFORE/AFTER INTERACTIVE SLIDER ---
        const beforeContainer = document.getElementById('before-image-container');
        const sliderHandle = document.getElementById('slider-handle');
        const sliderParent = beforeContainer.parentElement;

        let isDragging = false;

        function setSliderPosition(clientX) {
            const rect = sliderParent.getBoundingClientRect();
            let offsetX = clientX - rect.left;
            let percentage = (offsetX / rect.width) * 100;

            if (percentage < 0) percentage = 0;
            if (percentage > 100) percentage = 100;

            beforeContainer.style.width = `${percentage}%`;
            sliderHandle.style.left = `${percentage}%`;
        }

        sliderHandle.addEventListener('mousedown', () => { isDragging = true; });
        window.addEventListener('mouseup', () => { isDragging = false; });
        sliderHandle.addEventListener('touchstart', () => { isDragging = true; });
        window.addEventListener('touchend', () => { isDragging = false; });

        window.addEventListener('mousemove', (e) => {
            if (!isDragging) return;
            setSliderPosition(e.clientX);
        });

        window.addEventListener('touchmove', (e) => {
            if (!isDragging) return;
            if (e.touches && e.touches[0]) {
                setSliderPosition(e.touches[0].clientX);
            }
        });

        // --- DYNAMIC REPAIR COST ESTIMATOR ---
        let currentBaseCost = 0;
        let currentMultiplier = 1.0;

        function selectEstimatorPanel(id, baseCost) {
            document.querySelectorAll('.panel-btn').forEach(btn => {
                btn.classList.remove('border-amber-400', 'bg-slate-900');
                btn.classList.add('border-slate-800', 'bg-slate-950');
            });
            event.currentTarget.classList.add('border-amber-400', 'bg-slate-900');
            event.currentTarget.classList.remove('border-slate-800', 'bg-slate-950');

            currentBaseCost = baseCost;
            calculateEstimatorResults();
        }

        function selectEstimatorSeverity(id, multiplier) {
            document.querySelectorAll('.severity-btn').forEach(btn => {
                btn.classList.remove('border-amber-400', 'bg-slate-900');
                btn.classList.add('border-slate-800', 'bg-slate-950');
            });
            event.currentTarget.classList.add('border-amber-400', 'bg-slate-900');
            event.currentTarget.classList.remove('border-slate-800', 'bg-slate-950');

            currentMultiplier = multiplier;
            calculateEstimatorResults();
        }

        function calculateEstimatorResults() {
            if (currentBaseCost === 0) {
                document.getElementById('estimate-output').textContent = "Select panel above...";
                return;
            }

            const totalCenter = currentBaseCost * currentMultiplier;
            const minRange = Math.round((totalCenter * 0.9) / 10) * 10;
            const maxRange = Math.round((totalCenter * 1.15) / 10) * 10;

            let timeframe = "1 - 2 business days";
            if (currentMultiplier > 1.2 && currentMultiplier < 2.5) {
                timeframe = "2 - 4 business days";
            } else if (currentMultiplier >= 2.5) {
                timeframe = "5 - 8 business days (Involves panel replacement)";
            }

            document.getElementById('estimate-output').textContent = `$${minRange} - $${maxRange}`;
            document.getElementById('estimate-time').textContent = `⌛ Est. Repair Turnaround: ${timeframe}`;
        }

        // --- DYNAMIC INSURANCE CONCIERGE TOOL ---
        const insuranceGuidelines = {
            aaa: {
                title: "AAA Direct Claim Agreement",
                desc: "California Custom Collision is a trusted collision & paint partner for AAA Southern California claims. This means fast-tracked processing and simplified authorizations.",
                points: [
                    "✓ Direct electronic billing (zero paperwork hand-offs)",
                    "✓ Quick-claim photo appraisal integration on-site",
                    "✓ Coordinated rental car pickup arranged directly from 12th St"
                ]
            },
            geico: {
                title: "GEICO Claim Express Coordination",
                desc: "We work seamlessly with GEICO field appraisers to get your vehicle fully inspected, authorized, and moving quickly.",
                points: [
                    "✓ Instant electronic upload of supplements directly to GEICO portal",
                    "✓ OEM specification parts protection guidelines",
                    "✓ Streamlined same-day approvals on supplemental items"
                ]
            },
            statefarm: {
                title: "State Farm Claims Handled Simply",
                desc: "We work directly with State Farm agents throughout the Santa Clarita Valley to authorize repairs without unnecessary delays.",
                points: [
                    "✓ Simplified supplement authorizations on structural components",
                    "✓ Deductible waiver options processed seamlessly on eligible claims",
                    "✓ Lifetime alignment and paint coat restoration warranty"
                ]
            },
            progressive: {
                title: "Progressive Claim Integration",
                desc: "Simply hand over your Progressive claim number and our service writers will coordinate the entire repair project.",
                points: [
                    "✓ Advanced Progressive digital estimate processing",
                    "✓ Fast towing coordination to our secure 12th St facility",
                    "✓ Direct electronic reimbursement and payment collection"
                ]
            }
        };

        function selectInsuranceProvider(providerId) {
            document.querySelectorAll('.insurance-logo-btn').forEach(btn => {
                btn.classList.remove('border-amber-400', 'bg-slate-800');
                btn.classList.add('border-slate-800', 'bg-slate-900');
            });
            event.currentTarget.classList.add('border-amber-400', 'bg-slate-800');
            event.currentTarget.classList.remove('border-slate-800', 'bg-slate-900');

            const data = insuranceGuidelines[providerId];
            if (!data) return;

            const target = document.getElementById('insurance-detail-content');
            target.innerHTML = `
                <div class="space-y-4">
                    <span class="text-xs font-bold text-amber-400 tracking-widest uppercase block">Direct Billing Verified</span>
                    <h3 class="text-2xl font-bold text-white font-display">${data.title}</h3>
                    <p class="text-slate-300 text-sm leading-relaxed">${data.desc}</p>
                    <hr class="border-slate-800 my-4">
                    <ul class="space-y-3 text-sm text-slate-300">
                        ${data.points.map(pt => `<li>${pt}</li>`).join('')}
                    </ul>
                    <div class="pt-4">
                        <a href="#book-appointment" class="inline-flex items-center gap-2 bg-slate-950 border border-slate-800 text-slate-200 hover:text-white px-5 py-2.5 rounded-xl text-xs font-bold transition-all">
                            <span>Claim Consultation Appointment</span>
                            <span>→</span>
                        </a>
                    </div>
                </div>
            `;
        }

        // --- FAQ TOGGLES ---
        function toggleFaq(id) {
            const el = document.getElementById(id);
            const icon = document.getElementById(`${id}-icon`);
            if (el.classList.contains('hidden')) {
                el.classList.remove('hidden');
                icon.textContent = '−';
                icon.classList.add('rotate-180');
            } else {
                el.classList.add('hidden');
                icon.textContent = '+';
                icon.classList.remove('rotate-180');
            }
        }

        // --- BOOKING FORM & CUSTOM MODAL ---
        function handleFormSubmission(event) {
            event.preventDefault();
            document.getElementById('booking-modal').classList.remove('hidden');
        }

        function closeBookingModal() {
            document.getElementById('booking-modal').classList.add('hidden');
            document.getElementById('appointment-form').reset();
        }
    </script>
</body>
</html>
