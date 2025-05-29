<script lang="ts">
	// Components
	import UseCases from "$lib/components/layout/UseCases.svelte";
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CustomerCardHero from "$lib/components/layout/hero-sections/CustomerCardHero.svelte";
</script>

<CustomerCardHero
  centered={true}
  title="Every customer, fully understood"
  subtitle="Lapel creates a living digital twin of each relationship by unifying conversations, system data, and activity—so every interaction feels personal, seamless, and one step ahead."
  customers={[ 
    {
      name: "Jessica Lee",
      position: "Director of Customer Success",
      imageSrc: "/generated/image-a-confident-professional-woman-stands-in.webp"
    },
    {
      name: "Michael Tran",
      position: "COO",
      imageSrc: "/generated/image-a-smiling-businessman-is-in-a-tech-theme.webp"
    },
    {
      name: "Ashley Chen",
      position: "Head of Growth",
      imageSrc: "/generated/image-a-young-asian-woman-is-in-a-meeting-spac.webp"
    },
    {
      name: "Samantha Riley",
      position: "Product Manager",
      imageSrc: "/generated/image-a-cheerful-young-professional-woman-is-w.webp"
    },
    {
      name: "David Kim",
      position: "VP of Operations",
      imageSrc: "/generated/image-a-thoughtful-senior-executive-man-is-sea.webp"
    }
  ]}
/>
<LogoScroller
	label="Trusted by industry leaders"
	logoUrls={[
		"https://logo.clearbit.com/zendesk.com",
		"https://logo.clearbit.com/hubspot.com",
		"https://logo.clearbit.com/asana.com",
		"https://logo.clearbit.com/salesforce.com"
	]}
/>

<Summary
	title="What we do"
	text="Lapel is a Customer Operations Platform that creates a digital twin of every customer relationship. By unifying data from every team and system, it empowers organizations to deliver faster, more personal service across every customer touchpoint."
/>

<Testimonials
	testimonials={[
		{
			name: "Samira Halston",
			position: "Head of Customer Operations",
			company: "RelaySync",
			quote:
				"Lapel has cut our prep and follow-up work by over 50%. It feels like we got back hours every week to focus on genuine customer conversations instead of digging for details.",
			image: "/generated/image-a-confident-woman-in-a-contemporary-offi.webp"
		},
		{
			name: "Ezra Boateng",
			position: "Support Lead",
			company: "NovaSphere",
			quote:
				"Lapel’s unified view means fewer mistakes and faster responses. We’ve dropped our critical ticket risk by a third—our SLAs finally feel safe.",
			image: "/generated/image-a-focused-man-working-in-a-call-center-w.webp"
		},
		{
			name: "Meilin Chao",
			position: "VP of Finance",
			company: "Optiview",
			quote:
				"Before Lapel, reconciling contract and billing data cost us both money and time. We’ve since cut error-driven losses and our audit process is twice as fast.",
			image: "/generated/image-a-middle-aged-east-asian-woman-in-a-fina.webp"
		}
	]}
/>

<Features
	title="Features that set us apart"
	subtitle="The essentials powering world-class customer operations"
	features={[
		{
			title: "A real-time digital twin for every customer",
			description: "See every conversation, action, and touchpoint unified in a single, living customer record as it evolves."
		},
		{
			title: "Full context in every conversation",
			description: "Deliver truly personal, decisive service—no more wasting time piecing together data from separate tools."
		},
		{
			title: "Automate and extend with smart playbooks & APIs",
			description: "Trigger perfectly-timed actions or build custom experiences for any team with agentic playbooks and robust APIs."
		}
	]}
/>

<UseCases
	title="Use Cases"
	subtitle="Real-world applications for your business needs"
	useCases={[
		{
			title: "Proactive account risk management",
			description: "Lapel tracks every customer signal—from silent weeks to urgent tickets—so your team can spot risks early and act before accounts spiral.",
			image: "/generated/image-an-account-manager-in-a-modern-office-se.webp",
			link: {
				href: "/use-cases/account-risk-signals",
				label: "Learn more"
			}
		},
		{
			title: "Revenue expansion signals",
			description: "Automatically surface upsell and cross-sell opportunities based on product usage, support interactions, and customer comments in emails or calls.",
			image: "/generated/image-a-collaborative-workspace-bustling-with-.webp",
			link: {
				href: "/use-cases/expansion-signals",
				label: "Learn more"
			}
		},
		{
			title: "Fast onboarding for new account teams",
			description: "When ownership changes, Lapel gives new owners full visibility into every past meeting, decision, and priority—no digging or guessing.",
			image: "/generated/image-a-busy-office-environment-where-an-accou.webp",
			link: {
				href: "/use-cases/account-onboarding",
				label: "Learn more"
			}
		}
	]}
/>

<AboutTeaser />
<CallToAction
  title="Every customer interaction, fully informed"
  subtitle="No more hunting through tools"
  description="Lapel brings together all customer context into a single, real-time view—so your team can engage confidently, every time. Just seamless service and stronger customer relationships."
  imageSrc="/generated/image-a-cheerful-customer-success-manager-with.webp"
  callsToAction={[{ href: '/contact', label: 'Power every interaction with clarity', variant: 'primary' }]}
/>
