<script>
	import Cta from '../components/CTA.svelte';
	import Header from '../components/Header.svelte';
	import TimelineJobUpdate from '../components/TimelineJobUpdate.svelte';
	import TimelineUpdate from '../components/TimelineUpdate.svelte';
</script>

<main class="flex flex-col">
	<Header />
	<div class="container mx-auto max-w-screen-xl">
		<div class="container mx-auto max-w-screen-lg">
			<Cta />
		</div>
        <div style="margin-left:8%">
            
            <TimelineUpdate />
			<TimelineJobUpdate/>
            <TimelineUpdate />
            <TimelineUpdate />
        </div>
	</div>
</main>
