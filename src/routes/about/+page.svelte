<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Built by real engineers, not consultants",
			description: "We don't write slide decks—we write production-grade code. With over 17 years of engineering leadership, hands-on development, and technical writing, we've faced the challenges you're up against—and solved them in production."
		},
		{
			title: "Turn repeated questions into reusable knowledge",
			description: "Capture the \"why\" behind decisions, not just the \"what.\" We transform senior engineers' context into documented guidance that helps junior developers level up—without asking twice."
		},
		{
			title: "The AI-enhanced workflow developers actually want",
			description: "We don't reinvent your workflow—we improve it. Our tools surface relevant architectural context, practical documentation, and high-signal examples exactly when they're needed—in development and during reviews."
		}
	];
</script>

<SecondaryHero
	title="From code to clarity"
	subtitle="Real insights from real engineering"
	imageSrc="/generated/image-a-professional-software-engineer-sitting.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"After years leading engineering teams across multiple tech stacks and company stages, we saw the same patterns repeat: incomplete context, junior engineers re-asking architecture questions, and bottlenecks during code reviews. Technical knowledge lived in silos, slowing down entire teams and frustrating experienced engineers who found themselves answering the same questions over and over. We knew there had to be a better way to scale engineering expertise.",
		"Borozdin Tech transforms this challenge into opportunity by turning complex software engineering problems into actionable insights. Drawing from 17+ years of hands-on experience and 70+ technical articles, we've developed AI-enhanced workflows that help teams capture and share architectural decisions effectively. Starting with technical content creators, we're building systems that make engineering knowledge accessible, searchable, and immediately useful.",
		"Today, we're reaching 50,000+ developers monthly through dev.to articles and conference presentations, helping engineering managers reduce code review bottlenecks and scale their teams' technical understanding. Our unique combination of deep technical implementation experience and product-focused engineering leadership means we don't just understand the code—we understand how to build sustainable, scalable development practices that drive real business outcomes."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Engineering leadership."
	subtitle="Built by developers, for developers."
	stakeholders={[
		{
			name: "Mike Borozdin",
			position: "Founder & Software Engineer",
			bio: "17+ years of engineering leadership across multiple countries and tech stacks. Author of 70+ technical articles and active conference speaker.",
			image: "/generated/image-a-professional-software-engineer-in-a-mo.webp"
		}
	]}
/>

<StakeholderGrid
	stakeholderType="partner"
	title="Trusted by developers."
	subtitle="Featured across top development platforms"
	stakeholders={[
		{
			name: "Dev.to Community",
			image: "https://logo.clearbit.com/dev.to"
		},
		{
			name: "Conference Speaker",
			image: "/generated/image-a-group-of-diverse-professionals-engaged.webp"
		},
		{
			name: "Open Source",
			image: "/generated/image-a-group-of-individuals-collaborating-on-.webp"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Stop repeating the same code review explanations"
	subtitle="Transform knowledge silos into shared understanding"
	description="Join the engineering managers already reducing review bottlenecks and accelerating their teams with our AI-enhanced workflows. Turn your senior engineers' expertise into documentation that scales."
/>
