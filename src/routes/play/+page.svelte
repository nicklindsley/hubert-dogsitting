<script lang="ts">
	import Section from "$lib/components/Section.svelte";
</script>

<div>
	<Section
		title="Favorite Toys"
		items={[
			{
				content: "Bones",
				subItems: [],
			},
			{
				content: "Purple octopus",
				subItems: [],
			},
			{
				content: "Plastic orange ball",
				subItems: [],
			},
		]}
	/>
	<Section
		title="Favorite Games"
		items={[
			{
				content: "Hide & Seek",
				subItems: [
					`Tell him to "wait" or go to "place"`,
					"Go hide somewhere in the house",
					`Yell "Hubert come find me" and let him search for you`,
				],
			},
			{
				content: "Search",
				subItems: [
					"Hide his bone or treats in a blanket",
					`Point to the blanket and say "search"`,
					"He'll dig around in the blanket looking for his bone/treats",
				],
			},
			{
				content: "Wrestling",
				subItems: [
					"Use a toy and push him around. Don't be afraid to get in his face, he loves it",
				],
			},
			{
				content: "Monkey in the Middle",
				subItems: [
					"Each of you toss a ball/toy/bone back and forth and let Hubert run between you",
				],
			},
			"He likes to be chased, so simply chasing him with his bone/toy can be fun",
			"If it snows, you can toss snow balls around the yard and he'll chase after them",
			{
				content: "Nerf Ball",
				subItems: [
					"Stuff some treats and/or kibble in between the cracks in the nerf ball",
					"He'll usually carry this around from room to room",
				],
			},
			{
				content: "Puzzle",
				subItems: [
					"Sprinkle some treats and kibble in each compartment",
					"He can be very loud while working on this as he scratches away",
				],
			},
		]}
	/>
</div>
