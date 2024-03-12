<script lang="ts">
	import Cta from '../components/CTA.svelte';
	import Header from '../components/Header.svelte';
	import TimelineJobUpdate from '../components/TimelineJobUpdate.svelte';
	import TimelineUpdate from '../components/TimelineUpdate.svelte';
	import TimelineUtil from '../components/TimelineUtil.svelte';
	import { onMount } from 'svelte';

	let data: any = undefined;

	onMount(async () => {
		const res = await fetch(
			'https://gist.githubusercontent.com/shashankdaima/1c7123dc2d8a122fb02fd8aadd8202ea/raw/ebcfa85462a1e81d547164866eee10e46c7c1e89/response.json'
		);
		data = await res.json();
	});
</script>

<main class="flex flex-col">
	{#if data}
		<Header />
		<div class="container mx-auto max-w-screen-xl">
			<div class="container mx-auto max-w-screen-lg">
				<Cta
					profileImage={data.profile_photo}
					companyLogo={data.logo}
					name={data.name}
					role={data.position}
					company={data.company_name}
					bio={data.bio}
				/>
			</div>
			<div>
				{#each data.timeline as item}
					{#each item.checkpoints as checkpoint}
						<TimelineUpdate checkpoint={checkpoint} />
					{/each}
					<TimelineJobUpdate job={item} />
				{/each}
			</div>
		</div>
	{:else}
		<p>Loading...</p>
	{/if}
</main>
