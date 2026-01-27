<script lang="ts">
	import Section from "$lib/components/Section.svelte";

	type Event = { time: string; description: string; subItems?: string[] };

	const events: Event[] = [
		{
			time: "7 - 8 AM",
			description:
				"Wake up and take him potty. He usually won't get up until you get up. He will typically poop in the morning but not always.",
		},
		{ time: "8 AM", description: "Playtime. He'll have a burst of energy after going potty." },
		{
			time: "8 - 9 AM",
			description: "Breakfast. Playtime helps build his appitite.",
			subItems: [
				"Try to get him to eat at least a little bit. Sometimes if he doesn't eat anything by 12-2 PM he'll throw up",
			],
		},
		{
			time: "5 - 10 PM",
			description:
				"Dinner. He eats very late sometimes, even right before bed. It never seems to affect him or cause him to get up in the middle of the night so we let him eat",
		},
		{
			time: "30 Minutes Before Bed",
			description:
				"Limit his water so he doesn't have to get up in the middle of the night. A little water is fine, but no big drinks",
		},
		{
			time: "Before Bed",
			description:
				"Take him out one last time before bed. Give him a chance to poop, especially if he hasn't pooped twice yet, but if he doesn't its usually not an issue.",
		},
	];
</script>

<div>
	<Section
		title="A day in the life of Hubert"
		items={events.map((e) => ({
			content: `<span><strong>${e.time}</strong> – ${e.description}</span>`,
			subItems: e.subItems,
		}))}
	/>
</div>
