<script lang="ts">
	import type { ComponentProps } from "svelte";
	import { hubertSleeping } from "$lib/assets";
	import Section from "$lib/components/Section.svelte";

	const sections: (ComponentProps<typeof Section> & { side: "left" | "right" })[] = [
		{
			title: "Meals",
			side: "left",
			items: [
				"He doesn't have specific meal times. We leave food out for him and he eats when he wants.",
				"If he eats between 1/2 - 1 cup of food a day that's good. The more the better. If he does eat all the food in his bowl/puzzle refill it. He probably won’t eat it right away, but we never limit the amount of kibble we give him in a day.",
				{
					content:
						"The most important thing is that he eats something in the morning. Breakfast is the hardest meal to convince him to eat, but the most important. He will sometimes throw up yellow flem if he doesn't eat anything by around lunch time.",
					subItems: [
						"We will give him some frozen food in the morning as he usually likes that. If he only eats that, it's usually enough that he won't puke.",
						"If if he won't eat by 11 AM you can mix some treats in with his kibble just to get him to eat something.",
					],
				},
				"As long as he eats something in the morning, we just leave food out for him and he'll eventually eat some more throughout the day.",
				"If he does puke, give him some of the frozen pumpkin and frozen kibble pieces – he gobbles up the pumpkin and it should settle his tummy.",
				{
					content:
						"He has a variety of food puzzles that he might find more interesting than a bowl.",
					subItems: [
						"Pupsicle – just pop a frozen ball and screw it closed. If he doesn’t finish it in 1 sitting, refrigerate any leftovers.",
						"Puzzles – fill each section with kibble and a piece of a treat.",
						"It helps to do a bit of play to work up his appetite.",
					],
				},
				"He may shake if he hasn't eaten in a long while (or he's cold). This is usually an indicator that he should eat",
				{
					content:
						"We gave you two filled Kongs. You can give Hubert one of these for breakfast or dinner. He will likely eat the entire thing, but might need some help getting the last little bit out.",
					subItems: [
						"If he doesn't eat it all, put it back in the freezer.",
						"If you want to make more, add 1/2 cup of kibble with 1/2 cup of water and let soak in the fridge for 3 hours (?? need to confirm time). Then stuff Kongs (with a couple treats mixed throughout) and put in freezer till you want to use them. Give him any leftover wet kibble at his next meal.",
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
						"His favorite toy is the purple octopus, but he obsesses over it. Break this out if you really need to burn some energy, but that will be the only toy he cares about.",
						"He loves his bones. He will chew them on his own, he’ll run around with them in his mouth, you can *carefully* throw them, or you can hide them under a blanket for him to find.",
						"His all time favorite toy is the hard orange ball. This toy turns him into another dog. It gives him SO much energy, all the time. He looses his off button with this. He also turn into a cat with this toy. You can add food to it, but he prefers it empty. Just put it on the ground and he will whip that ball around and smack it into your base shoe. We gave this to you as a LAST resort - only if he seems really sad/too much energy/you guys don't know what to do.",
					],
				},
				{
					content: "Favorite games:",
					subItems: [
						"Keep away with a bone",
						"Wrestling (with or without a toy)",
						"Monkey in the middle with a toy or bone",
						"He likes to be chased",
						"If it snows, you can throw snow balls and he'll chase them",
						'Hide and Seek. Tell him to wait (in his bed or somewhere) and go hide behind a door, in a closet, in a dark room, etc. Then yell "Hubert, come find me!". You might have to repeat yourself a couple times. If you hear him getting close, be quiet. Eventually he should sniff you out (sometimes he forgets to use his nose and just listens for you). But then he\'ll get excited! We do this to help tire him out mentally.',
						"Snuffle mat or puzzle with treats hidden. Sprinkle a couple treats covered with a handful of kibble in either and let Hubert go to town.",
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
				"He loves walks! We don’t take him on walks every day, so he doesn’t expect/need one every day. But he loves them! Normally we’ll go for a 1-2 mile walk.",
				"Use his blue harness for walks and clip it in the front. It helps him read the leash and stay in line. However if it's cold and you put his red jacket on, you can just use the back clips on there - he might pull a little more, but he'll be fine.",
				{
					content:
						"If its snowy or muddy, you can put his boots on. They can be tricky to get on so if you can't you can skip them. Just wipe his feet with a wet wipe afterwards.",
					subItems: [
						"If you do use his boots, he will start out walking really slow like he can’t walk in his boots. He’s faking it. Give him a minute and he’ll practically be running.",
						`It's easiest to start putting on his front shoes. Then move onto the back. At the end, you can velcro the strap across his chest. Here's a video how to put shoes on: <a class="link" href="https://youtu.be/SRJ7irgFPy4?si=rjOUiFQha9_Gjdmm">https://youtu.be/SRJ7irgFPy4?si=rjOUiFQha9_Gjdmm</a>.`,
					],
				},
				{
					content:
						'He\'s still a puppy and gets distracted easily. Just give him a tug and say "come on".',
					subItems: [
						"Depending on the day, he will stop and stare at passing cars. Again, just pull him along.",
					],
				},
				"Don't be afraid to pull him along if you need to.",
				"Watch your feet because he tends to swerve back and forth and will walk right in front of your feet.",
				"He doesn't always pee or poop on walks.",
				"He might get the zoomies inside when you're back from a walk.",
			],
		},
		{
			title: "Potty",
			side: "left",
			items: [
				"He averages 2 poops a day, but 1 or 3 is not abnormal either - just depends how much he eats.",
				"Sometimes he poops when he’s excited (and he forgets he’s supposed to do that outside). So if you’re going somewhere new, just be aware that he might need to go.",
				"When it’s very cold, sometimes he stands in awkward positions and pees on his front paws. He will try to hide it and lick it clean when he comes inside – you can wipe it clean with a wet wipe.",
				{
					content: "He'll ring his bell when he needs to go out",
					subItems: [
						"If he's waiting by his bell, he might have rang it very quietly (or thinks he did).",
						"He'll also ring the bell if he's bored and wants to explore outside or wants a treat. So if he rings it excessively you don't need to take him out.",
						"He should only have to go potty every few hours – total a couple times per day. However the number of times he wants to go potty increase with the temperature.",
					],
				},
				{
					content:
						"Feel free to use the stake and black leash so you don't need to go out with him.",
					subItems: [
						"If he does his business and comes back he gets a treat. Otherwise don't treat him unless you want to spend all day standing by the door.",
					],
				},
			],
		},
		{
			title: "Bedtime",
			side: "left",
			items: [
				"We usually go to bed between 10-11pm, but Hubert will probably fall asleep on the couch before then.",
				"If he sleeps a lot during the afternoon and evening, it's helpful to have a little play session before bed to tire him out. If he had a busy day though, this isn't necessary.",
				"We roll the corners in on the bed blanket to create a homemade donut bed. He normally sleeps in that between our legs. However if he gets cold, he might come snuggle up by us. Just move him back to his bed and cover him up if you don’t want this.",
				"Occasionally he will wake up, shake off, come sniff us, and go back to bed. Don’t know why he does this, but it happens once every week or two. Doesn’t mean anything.",
				{
					content:
						"We do use white noise – it was originally for Hubert, but now we’re addicted to it. Feel free to use it if you want or if Hubert isn’t settling down.",
					subItems: [
						"There is a timer that will turn the white noise off. It happens when you quickly press the power button. You will see little lights on the bottoms for different times. Leave it on ♾️ and hold the power button down longer to turn it on and off.",
					],
				},
				"If Hubert has his collar on, we try to remember to take that off before bed.",
			],
		},
		{
			title: "Other",
			side: "right",
			items: [
				"Hubert is a follower. He will likely follow you everywhere you go. He should adapt his sleep schedule to whatever you want, so feel free to get up or go to bed at a different time.",
				"Hubert loves shoulder and butt scratches - sometimes he will just melt if you scratch in the right place :) He also loves licking us - he will lick you as long as you let him.",
				"Hubert gets boogers in his eyes, especially in the morning. He hates getting them taken out – we have to put him in a headlock. Don’t worry about them!",
				"He loves rabbit poop, but his tummy does not. We try to stop him or pick it out of his mouth if we see him chewing it. He’s fine to eat a couple pieces, but he will likely get some bad poops/puke if he eats too much, so be aware if you have rabbits in your yard.",
				"We gave you a few smelly t-shirts of ours. Break a new one out about every other day so Hubert has some fresh scents of ours.",
				{
					content:
						"Hubert will need to take his heartworm and tick medication on Friday, February 13.",
					subItems: [
						"He loves it like it’s a treat, we just try to give it to him after he’s eaten a little food.",
					],
				},
				"Hubert likes to make his bed when he comes to sit down by us on the couch, for example at night when we're relaxing. Sometimes this involves him digging, like he's trying to dig to China. Feel free to make him do that on one of our blankets so he doesn't ruin your blankets with his claws.",
				"When it’s time to settle down at night, sometimes he will lay between your legs, but other times he prefers to just lay in his bed by himself. If you want some snuggles, wait till he’s asleep, then you can scoop him up.",
			],
		},
		{
			title: "Understanding Hubert's Behavior",
			side: "left",
			items: [
				`<strong>Shaking/shivering:</strong> either cold or hungry. Put a sweatshirt on him and give him some food (frozen kibble if you need him to eat).`,
				`<strong>Sitting and staring at you:</strong> likely wants to play (or maybe snuggle). This is usually his way of begging for something. If you ignore him long enough, he might try to jump up by you or go ring the bell if he really wants to play. We continue to ignore him until he settles down - and then play :)`,
				`<strong>Waiting by the door:</strong> might need to go outside or wants to go outside and play`,
				`If he opens his mouth and rubs his teeth against your hand, he wants to wrestle and be pushed around. He loves rough play.`,
				`If he seems sassy like he’s barking at things or continually ringing the bell or just being annoying, he likely needs some mental stimulation and or a nap. We’d suggest spending a few minutes doing some tricks or giving him a puzzle with some treats and then putting him in timeout in his bed.`,
				`Hubert loves classic rock music.`,
			],
		},
	];

	const leftSections = sections.filter((s) => s.side === "left");
	const rightSections = sections.filter((s) => s.side === "right");
</script>

<div class="m-4 flex flex-col items-center gap-4">
	<img src={hubertSleeping} alt="Hubert sleeping" width={400} />
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
