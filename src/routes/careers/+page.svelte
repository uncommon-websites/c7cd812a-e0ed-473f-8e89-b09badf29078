<script lang="ts">
	// Types

	// Components
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Card from "$lib/components/ui/Card.svelte";
	import JobList, { type JobOpening } from "./JobList.svelte";

	// Icons
	import IconBriefcase from "~icons/lucide/briefcase";
	import IconUsers from "~icons/lucide/users";
	import IconHeart from "~icons/lucide/heart";
	import IconGlobe from "~icons/lucide/globe";

	// Constants
	const SECTION_BASE_CLASSES = "section-py section-px container mx-auto";
	const GRADIENT_BG_CLASSES =
		"bg-gradient-to-br from-gray-50 to-gray-100 dark:from-gray-900 dark:to-gray-800";
	const ICON_CONTAINER_CLASSES =
		"bg-primary-50 text-primary-600 dark:bg-primary-950 dark:text-primary-400 flex items-center justify-center rounded-full";

	const benefits = [
		{
			title: "Flexible Work",
			description: "Remote-first with flexible hours that respect work-life balance.",
			icon: IconBriefcase
		},
		{
			title: "Growth Opportunities",
			description: "Continuous learning with mentorship and education stipends.",
			icon: IconUsers
		},
		{
			title: "Comprehensive Benefits",
			description: "Health coverage, retirement plans, and generous paid time off.",
			icon: IconHeart
		}
	];

	const openings: JobOpening[] = [
		// Engineering
		{
			title: "Senior Frontend Developer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Backend Engineer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Design Engineer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Design
		{
			title: "UX/UI Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Product Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Product
		{
			title: "Product Manager",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Product Analyst",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Marketing
		{
			title: "Marketing Specialist",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Content Strategist",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Social Media Manager",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		}
	];

	const employeeTestimonials = [
  {
    name: "Kenji Mori",
    position: "Software Engineer",
    company: "Engineering Team",
    quote:
      "Every quarter, I find myself solving new engineering problems alongside folks from product, design, and customer success. The tight feedback loops and shared goal-setting mean I'm always learning and contributing where it actually matters.",
    image:
      "/generated/image-a-lively-office-setting-with-an-east-asi.webp"
  },
  {
    name: "Mariela Torres",
    position: "People Operations Manager",
    company: "HR & Culture Team",
    quote:
      "From day one, I felt seen and included—not just welcomed. Management puts real energy into supporting flexible work, creating space for feedback, and intentionally building a culture that actually reflects our values.",
    image:
      "/generated/image-a-latina-female-people-operations-manage.webp"
  },
  {
    name: "Aaliyah Brooks",
    position: "Customer Success Lead",
    company: "Customer Operations Team",
    quote:
      "When I started at Lapel, my manager helped craft a career path that matches my strengths and where I want to grow. I'm leading key accounts now, but the best part is knowing I'm part of a team where every customer really matters.",
    image:
      "/generated/image-a-professional-office-setting-with-a-bla.webp"
  }
];

	const processSteps = [
  {
    step: 1,
    title: "Apply online",
    description:
      "Share your resume or LinkedIn and why you're interested. No hoops, no busywork."
  },
  {
    step: 2,
    title: "Intro chat",
    description:
      "Meet a team member for a brief conversation. We want to learn about you and share more on the role."
  },
  {
    step: 3,
    title: "Skills & deep dive",
    description:
      "Tackle a relevant challenge or join us for a collaborative session—tailored to the role."
  },
  {
    step: 4,
    title: "Team fit & feedback",
    description:
      "Meet more of the team, ask questions, and receive clear, actionable feedback after every step."
  }
];

	const values = [
		{
			icon: IconHeart,
			title: "Passion",
			description: "We're driven by a shared passion for innovation and excellence."
		},
		{
			icon: IconUsers,
			title: "Collaboration",
			description: "We believe in teamwork and collaboration to achieve great things."
		},
		{
			icon: IconGlobe,
			title: "Global Impact",
			description: "We're committed to making a positive impact on the world."
		}
	];
</script>

<!-- Hero Section -->

<SecondaryHero
	title="Build the future of service"
	subtitle="Join a team where your work truly matters"
	imageSrc="/generated/image-a-diverse-team-of-professionals-collabor.webp"
/>

<!-- Why Join Us Section -->
<section class={SECTION_BASE_CLASSES}>
	<SectionHeader title="Why join us?" subtitle="Set new standards. Build real impact." />

<div class="mt-8 text-body text-emphasis-low max-w-3xl">
  <p>
    Lapel is redefining how teams operate by creating the foundation for connected, ambitious customer relationships at every scale. Every person here helps shape both what we build and how we grow.
  </p>
</div>

	<div class="mt-16 grid gap-4 md:grid-cols-3">
		{#each benefits as benefit}
			<Card {...benefit} />
		{/each}
	</div>
</section>

<!-- Culture Section -->
<Culture {values} />
<div class="mt-8 text-body text-emphasis-low max-w-3xl">
  <p>
    We care deeply about service, move quickly, and expect roles to grow fast with the company. Experimentation is encouraged and failure is considered essential learning. Culture here means trust, transparency, daily context, and fast, direct feedback—people are trusted to do their best work, every day.
  </p>
</div>

<Testimonials testimonials={employeeTestimonials} />

<!-- Application Process -->
<section class={SECTION_BASE_CLASSES}>
	<div class="mx-auto">
		<h2 class="text-title1 mb-16">Our application process</h2>
<div class="mb-8 text-body text-emphasis-low max-w-3xl">
  <p>
    We keep it simple and transparent. Youll always hear from us—fast feedback and actionable insights at every stage, no ghosting. Heres how it works:
  </p>
</div>

		<div class="grid gap-12 md:grid-cols-3">
			{#each processSteps as { step, title, description }, i}
				<div class="flex flex-col">
					<div class="{ICON_CONTAINER_CLASSES} mb-6 size-11">
						<span class="text-headline">{step}</span>
					</div>
					<h3 class="text-headline mb-3">{title}</h3>
					<p class="text-body text-emphasis-low">{description}</p>
				</div>
			{/each}
		</div>
	</div>
</section>
<!-- Current Openings Section -->
<section class={GRADIENT_BG_CLASSES}>
	<div class="section-px section-py container mx-auto grid w-full items-start lg:grid-cols-2">
		<SectionHeader title="Current openings" subtitle="Find your perfect role" />

		<JobList {openings} />
	</div>
</section>
