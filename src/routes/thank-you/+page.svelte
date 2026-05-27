<script lang="ts">
</script>

<svelte:head>
	<title>VAELIA | Thank You</title>
	<meta name="description" content="Thank you for your pilot access request." />
</svelte:head>

<div class="fixed inset-0 overflow-hidden pointer-events-none z-0">
	<div class="absolute -top-[40%] -left-[20%] w-[80%] h-[80%] rounded-full bg-brand-teal/5 blur-[120px] animate-pulse-glow"></div>
</div>

<div class="relative min-h-screen bg-brand-bg text-text-gray font-sans flex flex-col justify-between selection:bg-brand-teal selection:text-white z-10">
	
	<!-- Header / Nav -->
	<header class="border-b border-brand-card/50">
		<div class="max-w-7xl mx-auto px-6 h-20 flex items-center justify-between">
			<a href="/" class="flex items-center space-x-3 group">
				<div class="w-8 h-8 rounded-lg bg-brand-card border border-brand-teal/30 flex items-center justify-center font-display font-black text-brand-teal group-hover:border-brand-teal/80 transition-colors">
					V
				</div>
				<span class="font-display font-black tracking-widest text-xl text-off-white group-hover:text-brand-teal transition-colors">VAELIA</span>
			</a>
		</div>
	</header>

	<!-- Main content -->
	<main class="max-w-xl mx-auto px-6 py-24 text-center space-y-8 my-auto">
		<div class="w-16 h-16 rounded-full bg-brand-teal/10 border border-brand-teal/40 flex items-center justify-center mx-auto text-brand-teal">
			<svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
				<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M5 13l4 4L19 7"></path>
			</svg>
		</div>
		
		<h1 class="text-3xl sm:text-4xl font-extrabold text-off-white font-display">
			Request Received
		</h1>
		
		<p class="text-base text-text-gray leading-relaxed">
			Your request for pilot access has been submitted successfully. I review every submission personally to ensure a productive pilot cohort. You will receive a response within 1 business day.
		</p>
		
		<div class="pt-4">
			<a 
				href="/" 
				class="btn-primary"
			>
				Return Home
			</a>
		</div>
	</main>

	<!-- Footer -->
	<footer class="py-12 px-6 border-t border-brand-card/50 text-xs">
		<div class="max-w-7xl mx-auto flex flex-col md:flex-row items-center justify-between gap-6">
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
	</footer>

</div>
