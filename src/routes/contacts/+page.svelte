<script lang="ts">
	type PhoneNumber = `${number}-${number}-${number}`;
	type Contact = { name: string; phone: PhoneNumber; link?: string };

	const contacts: Contact[] = [
		{ name: 'Nick', phone: '920-264-6984' },
		{ name: 'Michaela', phone: '920-530-7838' },
		{ name: 'Penny McLeod', phone: '920-819-5517' },
		{ name: 'Sue Lindsley', phone: '920-819-1768' },
		{
			name: 'Animal House (Vet)',
			phone: '920-465-4629',
			link: 'https://www.animalhousegreenbay.com/service/urgent-care-2/',
		},
	];
</script>

<div>
	<div class="grid grid-cols-2 gap-x-8 gap-y-2">
		<p class="font-bold">Name</p>
		<p class="font-bold">Phone</p>
		{#each contacts as contact (contact.name)}
			{#if contact.link}
				<!-- eslint-disable-next-line svelte/no-navigation-without-resolve -->
				<a class="underline" href={contact.link}>{contact.name}</a>
			{:else}
				<p>{contact.name}</p>
			{/if}
			<p>{contact.phone}</p>
		{/each}
	</div>
	<p class="mt-3 italic">*Call Nick in case of emergency 24/7*</p>
</div>
