<!--
@component AboutTeaser
A minimalist teaser for the about page featuring the founder's story.
-->
<script lang="ts">
	// Types
	type TeamMember = {
		name: string;
		role: string;
		image: string;
	};

	// Components
	import Button from "../ui/Button.svelte";
	import ScrollText from "./sub/ScrollText.svelte";

	// State
	let sectionRef: HTMLElement;

	let props = $props();

	// Data
	const teamMember: TeamMember = {
		name: "Mike Borozdin",
		role: "Founder & Software Engineer",
		image: "/generated/image-a-professional-software-engineer-working.webp"
	};
</script>

<section bind:this={sectionRef} {...props}>
	<div class="section-px section-py container mx-auto">
		<div class="relative mx-auto grid max-w-2xl place-items-center gap-16">
			<ScrollText
				class="text-title1 text-center"
				text={`"After watching countless engineering teams struggle with the same architectural questions and technical debt patterns across four countries, I realized the problem wasn't technical complexity—it was knowledge transfer. That's when everything changed."`}
			/>

			<!-- Team Member & CTA Section -->
			<div class="grid items-center gap-8">
				<div class="flex items-center justify-center gap-4">
					<img
						src={teamMember.image}
						alt={teamMember.name}
						class="size-12 rounded-full object-cover"
					/>
					<div>
						<div class="text-callout">{teamMember.name}</div>
						<div class="text-caption text-emphasis-low">{teamMember.role}</div>
					</div>
					<Button href="/about" variant="secondary" size="sm" class="ml-8">Read the full story</Button>
				</div>
			</div>
		</div>
	</div>
</section>
