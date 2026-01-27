<script lang="ts">
	import type { ComponentProps } from "svelte";
	import { hubertSleeping } from "$lib/assets";
	import Section from "$lib/components/Section.svelte";

	const sections: ComponentProps<typeof Section>[] = [
		{
			title: "Meals",
			items: [
				"He doesn't have specific meal times. We leave food out for him and he eats when he wants",
				"If he eats between 1/2 - 1 cup of food a day that's good. The more the better.",
				{
					content:
						"The most important thing is that he eats something in the morning. He will sometimes throw up flem if he doesn't eat anything by early/mid afternoon",
					subItems: [
						"Do whatever you need to do to get him to eat (treats, tricks, frozen food)",
					],
				},
				{
					content:
						"He has a variety of food puzzles that he might find more interesting than a bowl",
					subItems: [
						"Pupsicle – just pop a frozen ball and screw it closed. If he doesn’t finish it in 1 sitting, refrigerate any leftovers",
						"Puzzles – fill each section with kibble and a piece of a treat",
					],
				},
				"It helps to do a bit of play to work up his appetite",
				"He may shake if he hasn't eaten in a long while (or hes cold). This is usually an indicator that he should eat",
			],
		},
		{
			title: "Walks",
			items: [
				"Use his blue harness for walks and clip it in the front. It helps him read the leash and stay in line",
				"If its snowy or muddy, you can put his boots on. They can be tricky to get on so if you can't you can skip them. Just wipe his feet with a wet wipe afterwards",
				{
					content:
						'He\'s still a puppy and gets distracted easily. Just give him a tug and say "come on"',
					subItems: ["Don't be afraid to pull him along if you need to"],
				},
				"Watch your feet because he tends to swerve back and forth and will walk right in front of your feet",
				"He doesn't always pee or poop on walks",
			],
		},
		{
			title: "Entertainment",
			items: [
				{
					content:
						"He's very happy watching out the window so that's an easy way to occupy him",
					subItems: [
						"If he barks too much feel free to shut the blinds or block him from the window",
					],
				},
				"If he gets too riled up and gets too nippy, just stop playing for a moment and he'll usually settle back down",
				{
					content: "His favorite toy is the purple octopus, but he obsesses over it",
					subItems: [
						"Break this out if you really need to burn some energy, but that will be the only toy he cares about",
					],
				},
				{
					content: "Favorite games",
					subItems: [
						"Keep away with a bone",
						"Wrestling with a toy",
						"Monkey in the middle with a toy or bone",
						"He likes to be chased",
						"If it snows, you can throw snow balls and he'll chase them",
					],
				},
			],
		},
		{
			title: "Potty",
			items: [
				"He averages 2 poops a day, but 1 or 3 is not abnormal either",
				{
					content: "He'll ring his bell when he needs to go out",
					subItems: [
						"If he's waiting by his bell, he might have rang it very quietly",
						"He'll also ring the bell if he's bored and wants to explore outside or wants a treat. So if he rings it excessively you don't need to take him out",
						"He should only have to go potty every few hours",
					],
				},
			],
		},
		{
			title: "Bedtime",
			items: [],
		},
		{
			title: "Other",
			items: [],
		},
		{
			title: "Understanding Hubert's Behavior",
			items: [],
		},
	];
</script>

<div class="m-4 flex flex-col items-center gap-4">
	<img src={hubertSleeping} alt="Hubert sleeping" width={400} />
	<div class="grid md:grid-cols-2">
		{#each sections as section (section.title)}
			<Section {...section} />
		{/each}
	</div>
</div>
