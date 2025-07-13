<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CenteredTextOnlyHero from "$lib/components/layout/hero-sections/CenteredTextOnlyHero.svelte";
</script>

<CenteredTextOnlyHero
	title="Transform complex software engineering challenges into actionable insights"
	subtitle="Scale your engineering team's knowledge and eliminate code review bottlenecks with practical solutions from 17+ years of hands-on experience across diverse technology stacks."
	imageSrc="/generated/image-a-serene-office-environment-with-a-group.webp"
	callsToAction={[
		{ href: "/about", label: "Learn about our approach" },
		{ href: "/contact", label: "Start a conversation" }
	]}
/>
<LogoScroller 
	label="Trusted by engineering teams at"
	logoUrls={[
		'https://cdn.brandfetch.io/stripe.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/figma.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/shopify.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/notion.so/w/400/h/400/logo'
	]}
/>

<Summary
	title="How we help engineering teams"
	text="Borozdin Tech transforms complex software engineering challenges into actionable insights for engineering managers at growing tech companies. We eliminate knowledge silos and reduce code review bottlenecks through practical solutions backed by 17+ years of hands-on experience across diverse technology stacks.

Our approach combines deep technical implementation expertise with product-focused engineering leadership to help your team scale technical knowledge effectively."
/>

<Testimonials
	testimonials={[
		{
			name: "Priya Sharma",
			position: "Engineering Manager",
			company: "ScaleWorks",
			quote:
				"Mike's architectural guidance reduced our code review cycle time from 3 days to 6 hours. Our junior developers now ask 70% fewer repetitive questions, and our deployment confidence has never been higher.",
			image: "/generated/image-a-confident-asian-woman-engineering-mana.webp"
		},
		{
			name: "Marcus Williams",
			position: "CTO",
			company: "DevFlow Labs",
			quote:
				"Working with Borozdin Tech eliminated our technical debt crisis. We saved over $180K in refactoring costs and reduced our critical bug count by 85% within 4 months.",
			image: "/generated/image-a-black-male-cto-standing-in-a-contempor.webp"
		},
		{
			name: "Carmen Rodriguez",
			position: "VP of Engineering",
			company: "InnovateTech",
			quote:
				"The knowledge transfer framework Mike implemented turned our team silos into a collaborative powerhouse. We're shipping features 40% faster with half the rework.",
			image: "/generated/image-a-happy-latina-woman-vp-of-engineering-i.webp"
		}
	]}
/>

<Features
	title="Engineering excellence through practical solutions"
	subtitle="Transform complex technical challenges into actionable outcomes with proven methodologies and hands-on expertise."
	features={[
		{
			title: "Technical debt resolution",
			description:
				"Systematically eliminate legacy code bottlenecks and architectural constraints that slow your team down. Our proven framework transforms messy codebases into maintainable systems that accelerate development velocity."
		},
		{
			title: "Engineering team scaling",
			description:
				"Scale your development capacity without sacrificing code quality or team cohesion. We establish knowledge-sharing practices and mentorship systems that eliminate recurring architectural questions."
		},
		{
			title: "Multi-stack expertise",
			description:
				"Navigate complex technology decisions with confidence across .NET, Java, JavaScript, Python, and modern frameworks. Our cross-platform experience prevents costly technology migrations and integration failures."
		},
		{
			title: "Production-ready implementations",
			description:
				"Deliver battle-tested code examples and architectural patterns from real client transformations. Every solution is validated in production environments, not theoretical concepts."
		},
		{
			title: "Leadership development",
			description:
				"Develop engineering leadership skills that drive both technical excellence and business results. Our approach combines hands-on coding experience with strategic product thinking."
		},
		{
			title: "Knowledge transfer systems",
			description:
				"Eliminate knowledge silos and reduce code review bottlenecks through systematic documentation and team education. Create self-sufficient teams that maintain high standards independently."
		}
	]}
/>
<AboutTeaser />
<CallToAction 
	title="Engineering clarity starts here"
	subtitle="Your team's technical questions shouldn't stall velocity"
	description="Scale your engineering judgment without repeating answers or clogging code reviews. We don't just make plans—we ship production-tested code that turns strategy into results. Built by engineers who've scaled teams and systems across 17+ years."
	imageSrc="/generated/image-a-confident-engineering-manager-smiling-.webp"
	callsToAction={[
		{ href: "/contact", label: "Book your free strategy session", variant: "primary" },
		{ href: "/about", label: "See how we work", variant: "secondary" }
	]}
/>
