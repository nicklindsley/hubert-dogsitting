<script lang="ts">
	import Section from "$lib/components/Section.svelte";

	type Event = { time: string; description: string; subItems?: string[] };

	const events: Event[] = [
		{
			time: "7 - 8 AM",
			description:
				"Wake up and take him potty. He doesn't get up until we get up, but he might be more excited or anxious and want to get up earlier. I doubt that if he does want to get it that it's because he needs to go outside. He loves to stretch and get some butt scratches in right away when he gets out of bed. He will typically poop in the morning but sometimes it doesn’t happen on the first trip outside.",
		},
		{
			time: "8 AM",
			description: "Playtime. He usually has a burst of energy after going potty.",
		},
		{
			time: "8 - 9 AM",
			description: "Breakfast. Playtime helps build his appetite.",
			subItems: [
				"Try to get him to eat at least a little bit. Sometimes if he doesn't eat anything by 10AM - 12PM he'll throw up. See notes in “Meals”.",
			],
		},
		{
			time: "5 - 10 PM",
			description:
				"Dinner. He eats very late sometimes, even right before bed. It never seems to affect him or cause him to get up in the middle of the night so we let him eat.",
		},
		{
			time: "60 Minutes Before Bed",
			description:
				"Limit his water so he doesn't have to get up in the middle of the night. A little water is fine, but no big drinks.",
		},
		{
			time: "Before Bed",
			description:
				"Take him out one last time before bed. Give him a chance to poop, especially if he hasn't pooped twice yet, but if he doesn't its usually not an issue.",
			subItems: [
				`<strong>**</strong> The first night, give him plenty of time to explore your bedroom and guide him up and down the ottoman into your bed. He'll most likely want to explore everything before going to bed. If you lay in bed, eventually he will figure out it's not play time and come join you!`,
			],
		},
	];
</script>

<div>
	<Section
		title="A day in the life of Hubert"
		subTitle="*As you probably know, it might take a couple days for him to adjust to this schedule in a new house*"
		items={events.map((e) => ({
			content: `<span><strong>${e.time}</strong> – ${e.description}</span>`,
			subItems: e.subItems,
		}))}
	/>
</div>
