<script>
	import Cta from '../components/CTA.svelte';
	import Header from '../components/Header.svelte';
	import TimelineJobUpdate from '../components/TimelineJobUpdate.svelte';
	import TimelineUpdate from '../components/TimelineUpdate.svelte';
	import TimelineUtil from '../components/TimelineUtil.svelte';
</script>

<main class="flex flex-col">
	<Header />
	<div class="container mx-auto max-w-screen-xl">
		<div class="container mx-auto max-w-screen-lg">
			<Cta />
		</div>
        <div >
            <TimelineUpdate />
			<TimelineJobUpdate/>
            <TimelineUpdate />
            <TimelineUpdate />
        </div>
	</div>
</main>
