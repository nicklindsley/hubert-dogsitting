<script lang="ts">
	import type { ComponentProps } from "svelte";
	import { blanketBed } from "$lib/assets";
	import Section from "$lib/components/Section.svelte";

	const sections: (ComponentProps<typeof Section> & { side: "left" | "right" })[] = [
		{
			title: "Meals",
			side: "left",
			items: [
				"He doesn't have specific meal times. We leave food out for him and he eats when he wants.",
				{
					content:
						"If he eats between 1/2 - 1 cup of food a day that's good. The more the better.",
					subItems: [
						"If he does eat all the food in his bowl/puzzle refill it.",
						"He probably won’t eat it right away, but we never limit the amount of kibble we give him in a day.",
					],
				},
				{
					content: "The most important thing is that he eats something in the morning.",
					subItems: [
						"Give him some frozen food in the morning and he should eat that without any fuss. If that's all he eats, that's enough.",
						"Theres a chance he will throw up yellow flem if he doesn't eat anything by the middle of the day (usually if he's eaten some rabbit poop that upsets him stomach).",
						"If he refuses to eat in the morning you can try a different flavor of kibble or mix some treats in just to get him to eat something.",
						"If he does puke, give him some of the frozen pumpkin and frozen kibble pieces – he gobbles up the pumpkin and it'll settle his tummy.",
					],
				},
				"As long as he eats a few bites in the morning, we just leave food out for him and he'll eventually eat some more throughout the day.",
				"We gave you 3 different flavors of kibble. The beef is his favorite so start with that, but feel free to rotate the flavors if he loses interest",
				{
					content:
						"He has a variety of food puzzles that he might find more interesting than a bowl.",
					subItems: [
						"Puzzles – fill each section with kibble and a piece of a treat.",
						"It helps to do a bit of play to work up his appetite.",
					],
				},
				{
					content:
						"We gave you two filled Kongs. You can give Hubert one of these for breakfast or dinner. He will likely eat the entire thing, but might need some help getting the last little bit out.",
					subItems: [
						"If he doesn't eat it all, put it back in the freezer.",
						"If you want to make more, add 1/2 cup of kibble with 1/2 cup of water and let soak in the fridge for 2-3 hours. Then stuff Kongs with the wet food and a couple treats mixed throughout, then put in freezer till you want to use them. Give him any leftover wet kibble at his next meal.",
					],
				},
			],
		},
		{
			title: "Entertainment",
			side: "right",
			items: [
				{
					content:
						"He's very happy watching out the window so that's an easy way to occupy him.",
					subItems: [
						"If he barks too much feel free to shut the blinds or block him from the window.",
					],
				},
				{
					content: "Toys:",
					subItems: [
						"He loves his bones. He will chew them on his own, he’ll run around with them in his mouth, you can throw them, or you can hide them under a blanket for him to find.",
						"His favorite plush toy is the purple octopus, but he obsesses over it and will only want to play with it over other toys. Break this out if you really need to burn some energy.",
						"His all time favorite toy is the hard orange ball. This toy turns him into a monster. He goes nuts and looses his off button as long as it's in play. You can put food in it or just leave it empty, but watch out because he will whip that ball around and smack it into your base shoe. This is our last resort toy that we only break out when he has tons of energy.",
					],
				},
				"If you guys are all bored and looking for something to do, Hubert loves exploring Wet Nose Bistro (over by Fleet Farm). Going there will likely tire him out from smelling everything in there!",
				"If he gets too riled up and gets too nippy/barking, just freeze and stop playing for a moment and he'll usually settle back down",
			],
		},
		{
			title: "Walks",
			side: "right",
			items: [
				"He loves walks! We only walk him every few days, so he doesn’t expect/need one every day. Normally we’ll go for a 1-2 mile walk (dependent on weather).",
				{
					content: "Use his red jacket harness and the blue leash.",
					subItems: ["Theres poop bags attached to the leash"],
				},
				{
					content:
						"If its snowy or muddy, you can put his boots on. They can be tricky to get on so you can skip them if its too much trouble. Just wipe his feet with a wet wipe afterwards to get any road salt or mud off.",
					subItems: [
						`It's easiest to start putting on his front shoes. Then move onto the back. At the end, you can velcro the strap across his chest. Here's a video how to put shoes on: <a class="link" href="https://youtu.be/SRJ7irgFPy4?si=rjOUiFQha9_Gjdmm">https://youtu.be/SRJ7irgFPy4?si=rjOUiFQha9_Gjdmm</a>.`,
						"If you do use his boots, he will start out walking slow but he'll pick up the pace after a min or so.",
					],
				},
				{
					content:
						'He\'s still a puppy and gets distracted easily. Just give him a tug and say "come on".',
					subItems: [
						"Depending on the day, he will stop and stare at passing cars/people/dogs. Again, just pull him along.",
						"You can bring some mini pork treats along to keep his focus if it becomes a problem",
					],
				},
				"He walks in front of us, but sometimes he'll stop suddenly to sniff or look at something.",
				"He doesn't always pee or poop on walks.",
				"He might get the zoomies inside when you're back from a walk.",
			],
		},
		{
			title: "Potty",
			side: "left",
			items: [
				"He averages 1-2 poops a day, but 3 is not abnormal either - just depends how much he eats.",
				{
					content:
						"He rings his bell when he needs to go out. Show him where it is and what door to go to. It might take him a bit to learn where it is, but he should catch on quick",
					subItems: [
						"If he's waiting by his bell, he might have rang it very quietly (or thinks he did).",
						"He should only have to go potty every few hours – a couple times per day in total.",
						"He'll also ring the bell if he's bored and wants to explore outside or wants a treat. So if he rings it excessively you don't need to take him out.",
						"If its nice outside, he'll probably ring the bell more just to explore.",
					],
				},
				{
					content:
						"Feel free to use the stake and black leash so you don't need to go out with him.",
					subItems: [
						"If he does his business and comes back he gets a treat. Otherwise don't treat him unless you want to spend all day letting him out.",
					],
				},
				"He loves rabbit poop, but his tummy does not. We try to stop him or pick it out of his mouth if we see him chewing it. He’s fine to eat a couple pieces, but he will likely get sick and puke if he eats too much, so be aware if you have rabbits in your yard.",
			],
		},
		{
			title: "Bedtime",
			side: "left",
			items: [
				"We usually go to bed between 10-11pm, but Hubert will probably fall asleep on the couch before then.",
				"If he sleeps a lot during the afternoon and evening, it's helpful to have a little play session before bed to tire him out. If he had a busy day though, this isn't necessary.",
				{
					content:
						"Put the black/white blanket on your bed and bunch the edges up to create a donut bed. He normally sleeps in that by our legs, but place it where ever you like.",
					subItems: [
						"If he gets cold, he might come snuggle up by you. Just move him back to his bed and cover him up if you don’t want this.",
						`<img src="${blanketBed}" width="200" />`,
					],
				},
				"Occasionally he will wake up, shake off, come sniff us, and go back to bed. Don’t know why he does this, but it doesn’t mean anything.",
				{
					content:
						"We use white noise for ourselves. Feel free to use it if you want or if Hubert isn’t settling down.",
					subItems: [
						"There is a timer that will turn the white noise off. It happens when you quickly press the power button. You will see little lights on the bottoms for different times. Leave it on ♾️ and hold the power button down longer to turn it on and off.",
					],
				},
				"We usually take his collar off before bed.",
				"He should adapt his sleep schedule to whatever you want, so feel free to get up or go to bed at a different time.",
				{
					content:
						"If he's licking his thighs/crotch a lot at night you can put his black body suit on before bed",
					subItems: [
						"Put his front legs through the holes, velcro along his back, and button behind his legs around his tail",
						"He's not a fan of wearing it and he'll move around initially to get comfortable in it, but he should sleep just fine",
					],
				},
			],
		},
		{
			title: "Staying Home Alone",
			side: "right",
			items: [
				"We always set up the playpen pieces with a blanket or rug on the floor, so he's semi contained.",
				"We always turn on white noise and/or classic rock music at a pretty loud volume. It helps him relax.",
				"Make sure he goes potty and possibly poop before you leave",
				"We try to exercise him before we leave to encourage him to nap",
				"As you leave, give him a few salmon treats (the high value ones). Give him a few more when you come back",
			],
		},
		{
			title: "Other",
			side: "right",
			items: [
				"The skin on his thighs is dry and he's been licking it lately, which just makes it worse. Try to stop him from doing this if you notice it",
				"Hubert loves shoulder and butt scratches - sometimes he will just melt if you scratch in the right place :) He also loves licking us - he will lick you as long as you let him.",
				"Hubert gets boogers in his eyes, especially in the morning. He hates getting them taken out. Don’t worry about them!",
				"We gave you a few used t-shirts of ours. Break a new one out every couple days so Hubert has some fresh scents of ours.",
				{
					content:
						"Hubert will need to take his heartworm and tick medication on Friday, February 13.",
					subItems: [
						"He loves it like it’s a treat, we just try to give it to him after he’s eaten a little food.",
					],
				},
				"Hubert likes to make his bed when he comes to sit down by us on the couch, for example at night when we're relaxing. Sometimes this involves him digging, like he's trying to dig to China. Feel free to make him do that on one of our blankets so he doesn't ruin your blankets with his claws.",
				{
					content:
						"He generally likes to lay between your legs on the couch or in his donut bed.",
					subItems: [
						"If you want some snuggles, wait till he’s asleep, then you can scoop him up.",
					],
				},
				{
					content: "Rides",
					subItems: [
						"He'll lay on your lap, but we like to bring his donut bed for longer rides so more comfortable for everyone",
						"He likes to look outside for a little bit and then he'll lay down and nap",
					],
				},
				"Hubert loves classic rock music.",
			],
		},
		{
			title: "Understanding Hubert's Behavior",
			side: "right",
			items: [
				`<strong>Shaking/shivering:</strong> either cold or not feeling well. Put a sweatshirt on him and give him some food (frozen kibble if you need him to eat).`,
				`<strong>Sitting and staring at you:</strong> likely wants to play (or maybe snuggle). This is his way of begging for something. If you ignore him long enough, he might try to jump up by you or go ring the bell if he really wants to play. We continue to ignore him until he settles down - and then play :)`,
				`<strong>Waiting by the door:</strong> might need to go outside or wants to go outside and play`,
				`If he opens his mouth and rubs his teeth against your hand, he wants to wrestle and be pushed around. He loves rough play.`,
				`If he seems sassy like he’s barking at things or continually ringing the bell or just being annoying, he likely needs some mental stimulation and or a nap. We’d suggest spending a few minutes doing some tricks or giving him a puzzle with some treats and then putting him in timeout in his bed (the "place" command).`,
			],
		},
	];

	const leftSections = sections.filter((s) => s.side === "left");
	const rightSections = sections.filter((s) => s.side === "right");
</script>

<div class="m-4 flex flex-col items-center gap-4">
	<div class="grid gap-3 md:grid-cols-2">
		<div class="flex flex-col gap-3">
			{#each leftSections as section (section.title)}
				<Section {...section} />
			{/each}
		</div>
		<div class="flex flex-col gap-3">
			{#each rightSections as section (section.title)}
				<Section {...section} />
			{/each}
		</div>
	</div>
</div>
