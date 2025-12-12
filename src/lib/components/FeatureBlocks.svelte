<script lang="ts">
	import FeatureBlock from './FeatureBlock.svelte';
</script>

<!-- Block 1: FlipAI Chat -->
<FeatureBlock 
	title="FlipAI Chat: Query 7 trillion rows instantly" 
	description="Natural language interface to query blockchain data across 30+ chains. Ask questions about wallets, transactions, protocols, and get instant insights."
	buttons={[
		{ text: "TRY FLIPAI CHAT", icon: true },
		{ text: "VIEW DOCS" }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm p-4 font-mono text-xs">
		<div class="flex items-center gap-2 border-b border-border pb-2 mb-4">
			<span class="text-accent">></span>
			<span class="text-muted">What are the top 10 wallets by ETH balance?</span>
			<span class="w-2 h-4 bg-accent animate-pulse"></span>
		</div>
		<div class="space-y-2">
			<div class="flex items-center gap-2 text-[10px] text-muted">
				<div class="w-2 h-2 bg-green-500 rounded-full"></div>
				Querying 7T rows across Ethereum mainnet...
			</div>
			<div class="h-2 bg-gray-100 w-3/4 rounded"></div>
			<div class="h-2 bg-gray-100 w-1/2 rounded"></div>
			<div class="h-2 bg-gray-100 w-5/6 rounded"></div>
		</div>
	</div>
</FeatureBlock>

<!-- Block 2: Agent-as-a-Service Platform -->
<FeatureBlock 
	title="Agent-as-a-Service: Automate your analytics" 
	description="Embed AI agents into your workflow via MCP, API, or Slack. Deterministic execution with 100% confidence in repeated operations."
	buttons={[
		{ text: "EXPLORE AGENTS", icon: true }
	]}
	alignRight={true}
>
	<div class="w-full max-w-md bg-white border border-border rounded shadow-sm p-6 flex flex-col gap-4">
		<div class="flex items-center gap-2 text-xs font-mono text-muted">
			<div class="w-4 h-4 border border-accent rounded-sm flex items-center justify-center">
				<div class="w-2 h-2 bg-accent rounded-[1px]"></div>
			</div>
			Agent analyzing on-chain activity...
		</div>
		<div class="w-full bg-gray-100 h-1.5 rounded-full overflow-hidden">
			<div class="bg-accent h-full w-2/3 animate-pulse"></div>
		</div>
		<div class="space-y-2 text-[10px] text-muted font-mono">
			<div class="flex items-center gap-2">
				<div class="w-2 h-2 bg-green-500 rounded-full"></div>
				DBT pipeline generated
			</div>
			<div class="flex items-center gap-2">
				<div class="w-2 h-2 bg-green-500 rounded-full"></div>
				Anomaly detection active
			</div>
			<div class="flex items-center gap-2">
				<div class="w-2 h-2 bg-accent rounded-full animate-pulse"></div>
				Monitoring metrics...
			</div>
		</div>
	</div>
</FeatureBlock>

<!-- Block 3: Dashboard Builder -->
<FeatureBlock 
	title="Dashboard Builder: From question to visualization" 
	description="Currently in beta. Build custom dashboards with natural language queries. AI generates the SQL, creates visualizations, and maintains the pipeline."
	buttons={[
		{ text: "JOIN BETA", icon: true }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm overflow-hidden font-mono text-[10px]">
		<div class="grid grid-cols-4 gap-2 p-2 border-b border-border bg-gray-50 text-muted">
			<div>CHAIN</div>
			<div>DAILY TXS</div>
			<div>ACTIVE WALLETS</div>
			<div>TVL (USD)</div>
		</div>
		{#each [
			{ chain: 'Ethereum', color: 'purple' },
			{ chain: 'Solana', color: 'blue' },
			{ chain: 'Avalanche', color: 'orange' },
			{ chain: 'Polygon', color: 'indigo' },
			{ chain: 'Arbitrum', color: 'blue' },
			{ chain: 'Optimism', color: 'red' }
		] as item, i}
			<div class="grid grid-cols-4 gap-2 p-2 border-b border-border/50 items-center">
				<div class="flex items-center gap-2">
					<div class="w-3 h-3 rounded-full bg-{item.color}-400/20"></div>
					<span class="text-{item.color}-600">{item.chain}</span>
				</div>
				<div class="h-1.5 w-12 bg-gray-100 rounded"></div>
				<div class="h-1.5 w-10 bg-gray-100 rounded"></div>
				<div class="h-1.5 w-14 bg-gray-100 rounded"></div>
			</div>
		{/each}
	</div>
</FeatureBlock>

<!-- Block 4: Address Intelligence & Anti-Sybil -->
<FeatureBlock 
	title="Address Intelligence: 700M wallets scored daily" 
	description="Comprehensive wallet labeling and scoring. Anti-Sybil detection for bot and farmer identification. Optimize airdrops and target real users."
	buttons={[
		{ text: "EXPLORE WALLET DATA", icon: true }
	]}
	alignRight={true}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm overflow-hidden font-mono text-[10px]">
		<div class="grid grid-cols-4 gap-2 p-2 border-b border-border bg-gray-50 text-muted">
			<div>WALLET</div>
			<div>LABEL</div>
			<div>RISK SCORE</div>
			<div>ACTIVITY</div>
		</div>
		{#each [
			{ label: 'Whale', risk: 'LOW', color: 'green' },
			{ label: 'Bot', risk: 'HIGH', color: 'red' },
			{ label: 'Active User', risk: 'LOW', color: 'green' },
			{ label: 'Farmer', risk: 'HIGH', color: 'red' },
			{ label: 'Protocol', risk: 'NONE', color: 'blue' },
			{ label: 'New User', risk: 'MED', color: 'yellow' }
		] as item, i}
			<div class="grid grid-cols-4 gap-2 p-2 border-b border-border/50 items-center">
				<div class="text-muted font-mono">0x{(i * 1234).toString(16).padStart(4, '0')}...</div>
				<div class="flex items-center gap-1">
					<div class="w-2 h-2 rounded-full bg-{item.color}-500"></div>
					<span class="text-{item.color}-600">{item.label}</span>
				</div>
				<div class="text-{item.color}-600 font-bold">{item.risk}</div>
				<div class="h-1.5 w-8 bg-gray-100 rounded"></div>
			</div>
		{/each}
	</div>
</FeatureBlock>

<!-- Block 5: Custom Agent Development -->
<FeatureBlock 
	title="Custom Agents: Built for your use case" 
	description="White-glove service with embedded PhD data scientists. Custom agent development and maintenance included with all partnerships."
	buttons={[
		{ text: "BOOK A DEMO", icon: true }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm p-4 flex flex-col gap-4">
		<div class="flex items-center justify-between border-b border-border pb-2">
			<div class="text-[10px] font-mono text-muted flex items-center gap-2">
				<span class="w-2 h-2 bg-green-500 rounded-full"></span>
				Custom Solutions Portfolio
			</div>
		</div>
		
		<!-- Agent Cards Grid -->
		<div class="grid grid-cols-2 gap-2">
			{#each [
				'Competitive Intelligence',
				'Airdrop Optimizer',
				'Validator Economics',
				'Dune Dashboard Query',
				'Wallet Targeting',
				'Custom Analytics'
			] as agent}
				<div class="border border-border rounded p-2 hover:border-accent transition-colors cursor-pointer">
					<div class="flex items-center gap-2 mb-1">
						<div class="w-2 h-2 bg-accent rounded-full"></div>
						<div class="text-[9px] font-bold">{agent}</div>
					</div>
					<div class="h-1 w-full bg-gray-100 rounded"></div>
				</div>
			{/each}
		</div>

		<div class="mt-auto space-y-2">
			<div class="flex items-center gap-2 text-[10px] text-muted font-mono">
				<span class="w-3 h-3 border border-accent rounded-full flex items-center justify-center text-[8px] text-accent">✓</span>
				PhD-embedded team support
			</div>
		</div>
	</div>
</FeatureBlock>
