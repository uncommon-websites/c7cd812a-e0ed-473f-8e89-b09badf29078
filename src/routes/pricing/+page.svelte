<script lang="ts">
	// Types
	import type { PageProps } from "./$types";

	// Components
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import Pricing from "$lib/components/layout/Pricing.svelte";

	// Props
	const { data }: PageProps = $props();
</script>

<Pricing />

<Testimonials
  testimonials={[
    {
      name: "Alina Zheng",
      position: "VP of Customer Experience",
      company: "Routeframe",
      quote:
        "With Lapel, we've gone from reactive chaos to actionable clarity. Our CS team understands each customer context instantly—and it shows in the feedback.",
      image: "/generated/image-a-professional-headshot-of-an-east-asian.webp"
    },
    {
      name: "Malik Owens",
      position: "Head of Commercial Ops",
      company: "Cloudbay",
      quote:
        "Before Lapel, prepping for a customer meeting felt like assembling a crime board. Now everything's just... there.",
      image: "/generated/image-a-professional-headshot-of-a-black-man-i.webp"
    },
    {
      name: "Julian Ramos",
      position: "Revenue Operations Lead",
      company: "Axtradium",
      quote:
        "Lapel became our single source of truth for every active deal and account. It's drastically reduced time spent reconciling systems—and boosted close rates, too.",
      image: "/generated/image-a-professional-headshot-of-a-latino-man-.webp"
    }
  ]}
/>

<CallToAction
	title="A shared brain for every customer relationship"
	subtitle="Lapel gives your entire team complete, real-time context on every account—so you can move faster, serve smarter, and never miss a moment."
	description="Start using Lapel today and power every touchpoint with everything your team needs. No more guessing, switching tabs, or digging for answers—just instant, trusted context where you need it. Ready to move faster?"
	imageSrc="/generated/image-a-happy-business-professional-in-a-moder.webp"
	callsToAction=[
		{ href: '/get-started', label: 'Get started', variant: 'primary' },
		{ href: '/contact', label: 'Talk to sales', variant: 'secondary' }
	]
/>
