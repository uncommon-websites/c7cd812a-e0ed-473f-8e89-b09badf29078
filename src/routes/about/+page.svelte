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
		title: "Unified by context",
		description: "We connect every customer touchpoint—across teams and tools—so everyone works from the same, real-time source of truth."
	},
	{
		title: "Clarity over noise",
		description: "We pursue deep customer understanding and reject the chaos of fragmented data, making every decision with full context."
	},
	{
		title: "Operate for impact",
		description: "Every initiative, workflow, and line of code is measured by the value it delivers to the teams and customers we serve."
	},
	{
		title: "Customer reality comes first",
		description: "Our digital twin reflects the real, living customer—not just static records. We build for accuracy, completeness, and trust."
	}
];
</script>

<SecondaryHero
	title="Every customer, fully connected"
	subtitle="A digital twin of every relationship so teams can deliver fast, consistent service at any scale"
	imageSrc="/mockups/airport-screen-1748477910196.png"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"We started in 2018 with a simple goal: make helpful tech that people actually need. While many chase profits, we chose to do things differently.",
		"Beyond making good products, we care about doing the right thing, being kind to our planet, and making sure everyone can use what we build. That's our compass.",
		"From day one, we've asked ourselves: 'Does this actually help people?' This question gets us through tough calls and shapes who we are. We're playing the long game here.",
		"We think about how our work affects real people's lives. We build tech that brings people together, keeps your information safe, and treats everyone fairly. When we stick to these basics, good things happen."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
  stakeholderType="team"
  title="Our team"
  subtitle="The people building Lapel's customer operations platform"
  stakeholders={[
    {
      name: "Alex Morgan",
      position: "Founder & CEO",
      bio: "Alex designs the architecture for Lapel’s customer operations platform and leads the vision for unified customer context across every team interaction.",
      image: "/generated/image-a-professional-headshot-of-a-man-in-busi.webp"
    },
    {
      name: "Jamie Chen",
      position: "Chief Design Officer",
      bio: "Jamie brings human-centered design to complex systems, ensuring Lapel is intuitive for every user and team.",
      image: "/generated/image-a-professional-headshot-of-a-woman-in-bu.webp"
    },
    {
      name: "Taylor Wright",
      position: "Head of Engineering",
      bio: "Taylor develops the infrastructure that powers Lapel—handling data at scale so every customer relationship stays accurate and actionable.",
      image: "/generated/image-a-professional-headshot-featuring-a-pers.webp"
    }
  ]}
/>

<StakeholderGrid
	stakeholderType="investor"
	title="Backed by the best."
	subtitle="Point Nine, TSIC and others"
	stakeholders={[
		{
			name: "Point Nine Capital",
			image: "https://cdn.brandfetch.io/pointnine.com/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7"
		},
		{
			name: "TSIC Ventures",
			image: "https://cdn.brandfetch.io/tiny.vc/w/400/h/400/logo?c=1a2b3c4d5e"
		},
		{
			name: "Sequoia Capital",
			image: "https://cdn.brandfetch.io/sequoiacap.com/w/400/h/400/logo"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="This is the foundation your team has been missing"
	subtitle="A real-time digital twin for every customer"
	description="Lapel gives ambitious teams a living digital twin of every customer relationship. Replace fragmented tools with a shared, real-time source of truth—and unlock service at scale, without the busywork. If you’re looking to unify your customer operations and break out of silos, start here."
	callsToAction={[
	  { href: '/get-started', label: 'Request early access', variant: 'primary' },
	  { href: '/contact', label: 'Talk to our team', variant: 'secondary' }
	]}
	imageSrc="/generated/image-a-modern-professional-b2b-team-leader-st.webp"
/>
