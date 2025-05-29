<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";

	let paragraphs = [
		"We started Lapel after seeing one too many teams struggle with the same problem—spending hours trying to understand what’s going on with a customer, only to realize no one had the full answer. Sales had part of the picture, support had another, and ops filled the gaps with spreadsheets and follow-ups. It slowed everything down and made great service harder than it needed to be.",
		"We believed the fix wasn’t just another dashboard, but a real foundation: software that could bring all those customer interactions into one complete, accurate view—accessible to everyone. So we built Lapel. A customer operations platform that creates a living, linked representation of each customer relationship, automatically stitched together from your systems, conversations, and data sources.",
		"Today, teams use Lapel to run faster, stay aligned, and treat every customer like their best one. It delivers instant context at every touchpoint across the customer lifecycle—so your team can work smarter, respond quicker, and focus on what matters: the relationship."
	];
</script>

<div class="">
	<article class="section-py container mx-auto grid max-w-full">
		<Summary text={paragraphs.join("\n\n")} />
	</article>
</div>
