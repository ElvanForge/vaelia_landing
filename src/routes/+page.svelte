<script lang="ts">
	import InquiryForm from '../components/InquiryForm.svelte';
</script>

<svelte:head>
	<title>VAELIA | Technical English for Systems & Logic</title>
	<meta name="description" content="Technical English training cohort optimized for software engineers, systems designers, and logic-driven professionals." />
</svelte:head>

<!-- Background glow decorations -->
<div class="fixed inset-0 overflow-hidden pointer-events-none z-0">
	<div class="absolute -top-[40%] -left-[20%] w-[80%] h-[80%] rounded-full bg-brand-teal/5 blur-[120px] animate-pulse-glow"></div>
	<div class="absolute top-[60%] -right-[10%] w-[60%] h-[70%] rounded-full bg-brand-teal/5 blur-[150px] animate-pulse-glow" style="animation-delay: -3s;"></div>
</div>

<div class="relative min-h-screen bg-brand-bg text-text-gray font-sans selection:bg-brand-teal selection:text-white z-10">
	
	<!-- Header / Nav -->
	<header class="sticky top-0 z-50 backdrop-blur-md bg-brand-bg/85 border-b border-brand-card/50 transition-all duration-300">
		<div class="max-w-7xl mx-auto px-6 h-20 flex items-center justify-between">
			<!-- Branding: Minimalist wordmark -->
			<a href="/" class="flex items-center space-x-3 group">
				<div class="w-8 h-8 rounded-lg bg-brand-card border border-brand-teal/30 flex items-center justify-center font-display font-black text-brand-teal group-hover:border-brand-teal/80 transition-colors">
					V
				</div>
				<span class="font-display font-black tracking-widest text-xl text-off-white group-hover:text-brand-teal transition-colors">VAELIA</span>
			</a>
			
			<nav class="flex items-center space-x-6 md:space-x-8 text-sm font-medium tracking-wide">
				<a href="#curriculum" class="hover:text-brand-teal transition-colors">Curriculum</a>
				<a href="#pilot" class="hover:text-brand-teal transition-colors">Pilot Program</a>
				<a href="#inquiry-section" class="hover:text-brand-teal transition-colors">Inquire</a>
			</nav>
		</div>
	</header>

	<!-- Hero Section -->
	<section id="hero" class="relative pt-12 pb-24 md:pt-24 md:pb-32 px-6 overflow-hidden">
		<div class="max-w-7xl mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
			
			<!-- Left column: Text Content -->
			<div class="lg:col-span-7 space-y-8 text-center lg:text-left">
				<div class="inline-flex items-center space-x-2 px-3.5 py-1.5 rounded-full bg-brand-teal/10 border border-brand-teal/30 text-xs font-semibold tracking-wider text-brand-teal animate-pulse">
					<span class="w-2 h-2 rounded-full bg-brand-teal"></span>
					<span>PILOT PROGRAM ENROLLMENT OPEN</span>
				</div>
				
				<h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold tracking-tight leading-none text-off-white font-display">
					VAELIA LANGUAGE <br class="hidden sm:inline" />
					<span class="text-gradient-emerald">CONSULTING</span>
				</h1>
				
				<p class="text-xl md:text-2xl font-light text-off-white max-w-2xl mx-auto lg:mx-0 leading-relaxed font-display">
					Technical English for Systems & Logic.
				</p>
				
				<p class="text-base md:text-lg text-text-gray max-w-xl mx-auto lg:mx-0 leading-relaxed">
					English communication training optimized for software developers, system architects, and technical analysts. Acquire the syntactic precision, vocabulary, and structural clarity required to document complex systems and coordinate engineering operations.
				</p>
				
				<div class="flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-4 pt-4">
					<a 
						href="#enrollment" 
						id="hero-enroll-cta"
						class="btn-primary w-full sm:w-auto text-center cursor-pointer"
					>
						Request Pilot Access
					</a>
					<a 
						href="#curriculum" 
						class="w-full sm:w-auto px-6 py-3 text-center border border-brand-card hover:border-brand-teal/50 hover:bg-brand-card/50 rounded-lg text-off-white font-display font-semibold transition-all duration-200"
					>
						Explore Curriculum
					</a>
				</div>
				
				<!-- Capacity indicators -->
				<div class="flex items-center justify-center lg:justify-start space-x-6 text-sm text-text-gray pt-2">
					<div class="flex items-center space-x-2">
						<svg class="w-4 h-4 text-brand-teal" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
							<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z"></path>
						</svg>
						<span>Starts July 1st</span>
					</div>
					<div class="w-1.5 h-1.5 rounded-full bg-brand-card"></div>
					<div class="flex items-center space-x-2">
						<svg class="w-4 h-4 text-amber-500" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
							<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0zm6 3a2 2 0 11-4 0 2 2 0 014 0zM7 10a2 2 0 11-4 0 2 2 0 014 0z"></path>
						</svg>
						<span>Limited to 5 seats.</span>
					</div>
				</div>
			</div>
			
			<!-- Right column: Showcasing Module Image -->
			<div class="lg:col-span-5 relative flex justify-center">
				<div class="relative w-full max-w-lg aspect-square glow-card bg-brand-card/30 p-4 border border-brand-card flex flex-col justify-between">
					
					<!-- Top code window bar -->
					<div class="flex items-center justify-between border-b border-brand-card/80 pb-3 mb-4">
						<div class="flex space-x-1.5">
							<div class="w-3 h-3 rounded-full bg-red-500/80"></div>
							<div class="w-3 h-3 rounded-full bg-yellow-500/80"></div>
							<div class="w-3 h-3 rounded-full bg-green-500/80"></div>
						</div>
						<div class="text-xs text-brand-teal/80 font-mono tracking-wider">parser_system.rs</div>
						<div class="w-4"></div>
					</div>
					
					<!-- Custom Visual representation -->
					<div class="relative flex-1 rounded-lg overflow-hidden bg-brand-bg/80 border border-brand-card flex items-center justify-center">
						<img 
							src="/images/module_1.png" 
							alt="Technical Syntax Logic Parse Tree Diagram" 
							class="max-w-full h-auto object-cover opacity-85 hover:opacity-100 transition-opacity duration-300"
						/>
						
						<!-- Overlay shadow gradient -->
						<div class="absolute inset-0 bg-gradient-to-t from-brand-bg via-transparent to-transparent pointer-events-none"></div>
						
						<!-- Tiny floating micro-element -->
						<div class="absolute bottom-4 left-4 bg-brand-bg/90 border border-brand-teal/40 rounded px-2.5 py-1 text-[10px] font-mono text-brand-teal backdrop-blur-md">
							syntax_engine.parse(input_parameters);
						</div>
					</div>
				</div>
			</div>
			
		</div>
	</section>

	<!-- The Pilot Offer Section -->
	<section id="pilot" class="py-24 px-6 bg-brand-card/10 border-t border-b border-brand-card/40">
		<div class="max-w-7xl mx-auto">
			<div class="text-center max-w-3xl mx-auto space-y-4 mb-16">
				<h2 class="text-3xl md:text-4xl font-bold tracking-tight text-off-white">Pilot Program Structure</h2>
				<div class="w-16 h-1 bg-brand-teal mx-auto rounded-full"></div>
				<p class="text-lg text-text-gray">
					A structured, interactive learning format designed for engineering professionals to build exactness and confidence in technical syntax translations.
				</p>
			</div>

			<!-- Center high-contrast card detailing the offer -->
			<div class="max-w-3xl mx-auto">
				<div class="glow-card bg-gradient-to-b from-[#1e293b] to-[#162032] p-8 md:p-12 relative overflow-hidden border border-brand-teal/20 shadow-2xl">
					
					<!-- Glow effect background -->
					<div class="absolute top-0 right-0 w-64 h-64 bg-brand-teal/10 rounded-full blur-3xl -mr-20 -mt-20 pointer-events-none z-0"></div>
					
					<div class="relative z-10 space-y-8">
						<div class="flex flex-wrap items-center justify-between gap-4 border-b border-brand-card/60 pb-6">
							<div>
								<span class="text-xs uppercase tracking-widest text-brand-teal font-semibold">MODULE 1 PILOT</span>
								<h3 class="text-2xl md:text-3xl font-bold text-off-white mt-1">Foundational Technical Syntax</h3>
							</div>
							<div class="text-right">
								<div class="text-3xl md:text-4xl font-extrabold text-off-white font-display">$150 <span class="text-sm font-normal text-text-gray">/ one-time</span></div>
								<span class="text-xs text-amber-500 font-mono">Limit 5 Students</span>
							</div>
						</div>

						<!-- Grid details of cohort structure -->
						<div class="grid grid-cols-1 sm:grid-cols-2 gap-6 text-sm">
							<div class="flex items-start space-x-3">
								<div class="p-2 rounded bg-brand-teal/10 border border-brand-teal/20 text-brand-teal mt-0.5">
									<svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
										<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z"></path>
									</svg>
								</div>
								<div>
									<h4 class="font-bold text-off-white">4-Week Intensive Cohort</h4>
									<p class="text-text-gray text-xs mt-1">Structured schedule containing live classes and interactive assignments.</p>
								</div>
							</div>
							
							<div class="flex items-start space-x-3">
								<div class="p-2 rounded bg-brand-teal/10 border border-brand-teal/20 text-brand-teal mt-0.5">
									<svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
										<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M12 4.354a4 4 0 110 5.292M15 21H3v-1a6 6 0 0112 0v1zm0 0h6v-1a6 6 0 00-9-5.197M13 7a4 4 0 11-8 0 4 4 0 018 0z"></path>
									</svg>
								</div>
								<div>
									<h4 class="font-bold text-off-white">Max 5 Students</h4>
									<p class="text-text-gray text-xs mt-1">Individualized session parameters to ensure thorough feedback for each participant.</p>
								</div>
							</div>

							<div class="flex items-start space-x-3">
								<div class="p-2 rounded bg-brand-teal/10 border border-brand-teal/20 text-brand-teal mt-0.5">
									<svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
										<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"></path>
									</svg>
								</div>
								<div>
									<h4 class="font-bold text-off-white">Starts July 1st</h4>
									<p class="text-text-gray text-xs mt-1">Scheduled sessions with direct instructor access.</p>
								</div>
							</div>

							<div class="flex items-start space-x-3">
								<div class="p-2 rounded bg-brand-teal/10 border border-brand-teal/20 text-brand-teal mt-0.5">
									<svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
										<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5c1.747 0 3.332.477 4.5 1.253v13C19.832 18.477 18.247 18 16.5 18c-1.746 0-3.332.477-4.5 1.253"></path>
									</svg>
								</div>
								<div>
									<h4 class="font-bold text-off-white">Includes Chapters 1-4 Coursebook</h4>
									<p class="text-text-gray text-xs mt-1">Complete digital manual containing structured grammar templates and logic tables.</p>
								</div>
							</div>
						</div>

						<!-- Benefit list -->
						<div class="border-t border-brand-card/60 pt-6 font-sans">
							<h4 class="font-display font-semibold text-off-white mb-4 text-sm tracking-wider uppercase">Key Objectives:</h4>
							<ul class="space-y-3.5 text-sm">
								<li class="flex items-center space-x-3">
									<svg class="w-5 h-5 text-brand-teal flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
										<path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path>
									</svg>
									<span>Convert architectural logic flowcharts into clear English explanations</span>
								</li>
								<li class="flex items-center space-x-3">
									<svg class="w-5 h-5 text-brand-teal flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
										<path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path>
									</svg>
									<span>Resolve lexical ambiguities in data schemas and software requirements</span>
								</li>
								<li class="flex items-center space-x-3">
									<svg class="w-5 h-5 text-brand-teal flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
										<path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path>
									</svg>
									<span>Structure logic constraints and error reports for multi-team alignment</span>
								</li>
							</ul>
						</div>

						<!-- Intermediate Navigation CTA -->
						<div class="pt-4 text-center">
							<a 
								href="#curriculum" 
								class="inline-flex items-center space-x-2 text-brand-teal hover:text-brand-teal-light font-display font-semibold tracking-wide transition-colors"
							>
								<span>View Curriculum</span>
								<svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
									<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M19 14l-7 7m0 0l-7-7m7 7V3"></path>
								</svg>
							</a>
						</div>

					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- Roadmap Section -->
	<section id="curriculum" class="py-24 px-6 max-w-7xl mx-auto">
		<div class="text-center max-w-3xl mx-auto space-y-4 mb-16">
			<span class="text-xs uppercase tracking-widest text-brand-teal font-semibold font-mono">CURRICULUM ROADMAP</span>
			<h2 class="text-3xl md:text-4xl font-bold tracking-tight text-off-white font-display">Evolution of Technical Logic</h2>
			<div class="w-16 h-1 bg-brand-teal mx-auto rounded-full"></div>
			<p class="text-lg text-text-gray">
				A modular progression path mapping language structures to computing architectures. Master each layer before scaling.
			</p>
		</div>

		<!-- 3-Column Grid -->
		<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
			
			<!-- Card 1: Module 1 -->
			<div class="glow-card flex flex-col justify-between h-full bg-brand-card/40 border border-brand-card">
				<div>
					<div class="relative h-48 overflow-hidden bg-brand-bg border-b border-brand-card flex items-center justify-center">
						<img 
							src="/images/module_1.png" 
							alt="Module 1: Code Syntax Analysis Diagram" 
							class="max-w-full h-auto object-cover opacity-80 hover:opacity-100 transition-opacity duration-300"
						/>
						<span class="absolute top-3 left-3 bg-brand-teal text-white text-[10px] font-mono font-bold tracking-wider px-2.5 py-1 rounded">
							NOW ENROLLING
						</span>
					</div>
					
					<div class="p-6 space-y-4">
						<div class="text-xs font-mono text-brand-teal font-bold tracking-wide">01 // FOUNDATION</div>
						<h3 class="text-xl font-bold text-off-white">Module 01: Systems & Infrastructure (The Pilot Cohort)</h3>
						<p class="text-sm text-text-gray leading-relaxed">
							Chapters 1–4. A comprehensive deep-dive into digital feedback loops, cloud-based tools, and automated machinery. Designed for B1+ Intermediate learners to master the technical lexicon and grammar—including Passive Voice and Conditionals—needed for high-stakes engineering communication.
						</p>
						<div class="text-xs font-mono text-brand-teal">Status: Now Enrolling.</div>
					</div>
				</div>
			</div>

			<!-- Card 2: Module 2 -->
			<div class="glow-card flex flex-col justify-between h-full bg-brand-card/40 border border-brand-card">
				<div>
					<div class="relative h-48 overflow-hidden bg-brand-bg border-b border-brand-card flex items-center justify-center">
						<img 
							src="/images/module_2.png" 
							alt="Module 2: System Architecture Diagram" 
							class="max-w-full h-auto object-cover opacity-80 hover:opacity-100 transition-opacity duration-300"
						/>
						<span class="absolute top-3 left-3 bg-[#1e293b] border border-brand-card text-brand-teal text-[10px] font-mono font-bold tracking-wider px-2.5 py-1 rounded">
							UPCOMING
						</span>
					</div>
					
					<div class="p-6 space-y-4">
						<div class="text-xs font-mono text-brand-teal font-bold tracking-wide">02 // DOCUMENTATION</div>
						<h3 class="text-xl font-bold text-off-white">Module 02: Advanced Automation & Reliability (Upcoming)</h3>
						<p class="text-sm text-text-gray leading-relaxed">
							Chapters 5–8. Advanced analysis of machine-to-machine communication, automated triage, and technical governance.
						</p>
						<div class="text-xs font-mono text-brand-teal">Status: Coming soon to Pilot graduates.</div>
					</div>
				</div>
			</div>

			<!-- Card 3: Module 3 -->
			<div class="glow-card flex flex-col justify-between h-full bg-brand-card/40 border border-brand-card">
				<div>
					<div class="relative h-48 overflow-hidden bg-brand-bg border-b border-brand-card flex items-center justify-center">
						<img 
							src="/images/module_3.png" 
							alt="Module 3: Code Review Collaboration Diagram" 
							class="max-w-full h-auto object-cover opacity-80 hover:opacity-100 transition-opacity duration-300"
						/>
						<span class="absolute top-3 left-3 bg-[#1e293b] border border-brand-card text-brand-teal/60 text-[10px] font-mono font-bold tracking-wider px-2.5 py-1 rounded">
							UPCOMING
						</span>
					</div>
					
					<div class="p-6 space-y-4">
						<div class="text-xs font-mono text-brand-teal font-bold tracking-wide">03 // LEADERSHIP</div>
						<h3 class="text-xl font-bold text-off-white font-display">Module 03: Sustainable Urban Strategy (Upcoming)</h3>
						<p class="text-sm text-text-gray leading-relaxed">
							Chapters 9–12. Exploration of green infrastructure modeling and policy-engineering interfaces.
						</p>
						<div class="text-xs font-mono text-brand-teal">Status: Coming soon to Pilot graduates.</div>
					</div>
				</div>
			</div>

		</div>
	</section>

	<!-- Direct Enrollment & Program Logistics Section -->
	<div id="enrollment" class="py-24 px-6 bg-brand-card/20 border-t border-brand-card/40 relative overflow-hidden">
		<div class="absolute bottom-0 right-0 w-[40%] h-[40%] bg-brand-teal/5 rounded-full blur-[100px] pointer-events-none z-0"></div>

		<div class="max-w-3xl mx-auto relative z-10 space-y-12">
			<!-- Enroll Block (where the old form used to be) -->
			<div class="glow-card bg-brand-card/50 p-8 border border-brand-card/85 shadow-lg text-center space-y-4">
				<a href="https://buy.stripe.com/6oUfZj2w7eFBevabk2bjW05" class="btn-enroll">Join the Founding Cohort - $150</a>
				<p class="founding-member-info">Founding Member Pilot (Module 01): $450 value, introductory price $150. Limited to 5 seats.</p>
			</div>

			<!-- Program Logistics Block -->
			<div class="glow-card bg-brand-card/50 p-8 border border-brand-card/85 shadow-lg space-y-6">
				<h2 class="text-2xl font-bold text-off-white font-display">Program Logistics</h2>
				<div class="w-16 h-1 bg-brand-teal rounded-full"></div>
				
				<div class="space-y-6 text-sm text-text-gray">
					<div class="space-y-1">
						<h3 class="font-bold text-off-white">Schedule</h3>
						<p class="leading-relaxed">
							Pilot Cohort Schedule: Tuesdays & Thursdays at 18:00 UTC+4. This window is optimized for global engineering teams across EMEA and South Asia. The program consists of 8 sessions (4 Technical Briefings and 4 Engineering Labs).
						</p>
					</div>
					<div class="space-y-1">
						<h3 class="font-bold text-off-white">Support</h3>
						<p class="leading-relaxed">
							Each Lab session includes a scaffolded 'Phrase Bank' to ensure you can participate in complex technical debates with confidence, regardless of your current English level.
						</p>
					</div>
					<div class="space-y-1">
						<h3 class="font-bold text-off-white">About Vaelia</h3>
						<p class="leading-relaxed">
							Engineered by a technical lead and curriculum developer, Vaelia provides a standardized framework for technical communication. We strip away general language 'filler' and focus exclusively on the precise syntax, professional lexicon, and boardroom dynamics required to operate at a native-level in high-stakes engineering environments.
						</p>
					</div>
				</div>
			</div>
		</div>
	</div>

	<InquiryForm />

	<!-- Footer -->
	<footer class="bg-brand-bg py-16 px-6 border-t border-brand-card/50 text-xs">
		<div class="max-w-7xl mx-auto flex flex-col items-center space-y-8">
			
			<!-- Footer CTA -->
			<div class="text-center space-y-4">
				<a 
					href="#enrollment" 
					class="btn-primary py-3.5 px-8 text-base cursor-pointer"
				>
					Request Pilot Access
				</a>
			</div>
			
			<div class="w-full flex flex-col md:flex-row items-center justify-between gap-6 pt-8 border-t border-brand-card/40">
				<div class="flex items-center space-x-3">
					<div class="w-6 h-6 rounded bg-brand-card border border-brand-teal/30 flex items-center justify-center font-display font-black text-brand-teal text-[10px]">
						V
					</div>
					<span class="font-display font-black tracking-widest text-sm text-off-white">VAELIA</span>
				</div>
				
				<div class="text-text-gray/65 text-center md:text-right">
					Vaelia Language Consulting is a subsidiary of Elvan Forge LLC. © 2026 Vaelia Language Consulting. All rights reserved.
				</div>
			</div>
			
		</div>
	</footer>

</div>
