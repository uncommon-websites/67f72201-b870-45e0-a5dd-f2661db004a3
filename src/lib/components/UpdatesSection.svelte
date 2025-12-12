<section class="py-20 border-b border-border">
	<div class="container-custom">
		<div class="grid grid-cols-1 md:grid-cols-2 gap-16">
			
			<!-- Left Column: CTA & Visual -->
			<div class="flex flex-col h-full">
				<div class="mb-8">
					<p class="font-mono text-xs text-muted mb-4">Get started</p>
					<h2 class="text-2xl font-medium mb-4">Blockchain intelligence for protocol teams</h2>
					<p class="text-muted font-light mb-8 text-sm leading-relaxed max-w-md">
						Flipside delivers PhD-curated data and embedded AI agents to automate your on-chain analytics. Focus on last-mile logic while we handle the first-mile complexity.
					</p>
					<div class="flex gap-3 mb-12">
						<button class="border border-border px-3 py-1.5 text-xs font-mono uppercase hover:bg-primary-50 transition-colors flex items-center gap-2">
							BOOK A DEMO
							<span class="text-muted border border-muted/30 rounded px-1 text-[9px] min-w-[16px] text-center">D</span>
						</button>
						<button class="border border-border px-3 py-1.5 text-xs font-mono uppercase hover:bg-primary-50 transition-colors flex items-center gap-2">
							TRY FLIPAI
							<span class="text-muted border border-muted/30 rounded px-1 text-[9px] min-w-[16px] text-center">F</span>
						</button>
					</div>
				</div>
				
				<!-- Blockchain Data Visual -->
				<div class="mt-auto w-full h-48 bg-gradient-to-br from-slate-900 to-slate-800 relative overflow-hidden flex items-center justify-center">
					<!-- Hexagonal grid pattern -->
					<div class="absolute inset-0" style="background-image: linear-gradient(30deg, rgba(255,255,255,0.05) 12%, transparent 12.5%, transparent 87%, rgba(255,255,255,0.05) 87.5%, rgba(255,255,255,0.05)), linear-gradient(150deg, rgba(255,255,255,0.05) 12%, transparent 12.5%, transparent 87%, rgba(255,255,255,0.05) 87.5%, rgba(255,255,255,0.05)), linear-gradient(30deg, rgba(255,255,255,0.05) 12%, transparent 12.5%, transparent 87%, rgba(255,255,255,0.05) 87.5%, rgba(255,255,255,0.05)), linear-gradient(150deg, rgba(255,255,255,0.05) 12%, transparent 12.5%, transparent 87%, rgba(255,255,255,0.05) 87.5%, rgba(255,255,255,0.05)); background-size: 80px 140px; background-position: 0 0, 0 0, 40px 70px, 40px 70px;"></div>
					
					<!-- Animated data streams -->
					{#each Array(20) as _, i}
						<div 
							class="h-full bg-gradient-to-t from-accent/30 to-transparent absolute" 
							style="
								left: {i * 5}%; 
								width: 2px; 
								opacity: {Math.random() * 0.5};
								animation: dataFlow {2 + Math.random() * 2}s ease-in-out infinite;
								animation-delay: {Math.random() * 2}s;
							"
						></div>
					{/each}
					
					<div class="absolute inset-0 flex items-center justify-center">
						<div class="bg-slate-900/90 text-white font-mono text-[10px] px-3 py-1.5 z-10 border border-accent/30">
							flipside.xyz
						</div>
					</div>
				</div>
			</div>

			<!-- Right Column: Updates -->
			<div>
				<p class="font-mono text-xs text-muted mb-8">Platform capabilities</p>
				
				<div class="space-y-12">
					<!-- Update 1 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">Foundation</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">Enterprise-grade curated data</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								7 trillion rows of on-chain data maintained and curated by PhD data scientists. 700 million labeled wallets scored daily for address intelligence. 30+ blockchain networks covered under one unified schema with direct Snowflake warehouse access.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Data Infrastructure</span>
						</div>
					</div>

					<!-- Update 2 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">Platform</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">Agent-as-a-Service infrastructure</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								Model Context Protocol (MCP) integration for IDE environments. API access for embedding agent capabilities into your services. Slack integration for conversational interfaces. Deterministic workflow execution with 100% confidence in repeated operations.
							</p>
							<div class="flex gap-2">
								<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">AI Agents</span>
								<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Automation</span>
							</div>
						</div>
					</div>

					<!-- Update 3 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">Solutions</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">Purpose-built AI applications</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								FlipAI Chat for querying 7 trillion rows. Dashboard Builder (beta) for custom visualizations. Anti-Sybil Detector for bot identification. Airdrop Optimizer for targeting real users. Competitive Intelligence Agent. Custom agent development service.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Products</span>
						</div>
					</div>

					<!-- Update 4 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">Partnership</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">White-glove embedded support</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								All partners receive access to full suite of purpose-built AI solutions. Custom agent development and maintenance included. Embedded PhD data scientist support model. Book a demo for white-glove onboarding.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Service Model</span>
						</div>
					</div>
				</div>
			</div>

		</div>
	</div>
</section>

<style>
	@keyframes dataFlow {
		0%, 100% { transform: translateY(100%); opacity: 0; }
		50% { opacity: 0.5; }
	}
</style>
