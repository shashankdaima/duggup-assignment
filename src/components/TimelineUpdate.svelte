<script lang="ts">
	import Card from './Card.svelte';
	import TimelineUtil from './TimelineUtil.svelte';
	export let checkpoint:any;
</script>

<!-- Timeline Container -->
<TimelineUtil>
	<div slot="timeline-left">
		<p class="text-gray-500 text-sm text-right mt-24 mr-4">{checkpoint.date}</p>
	</div>
	<div slot="timeline-marker">
		<div
			class="absolute top-24 left-1/2 -translate-x-1/2 flex justify-center items-center bg-blue-500 rounded-full w-5 h-5"
			style="margin-left: 1px;"
		>
			<div class="bg-white rounded-full w-3 h-3"></div>
		</div>
	</div>
	<div slot="body">
		<div class="grid grid-cols-1 md:grid-cols-2 gap-8 m-4 mr-12 ml-8 lg:mr-72">
			{#each checkpoint.items as i}
				<Card strokes={true}>
					<img
						src={i.image_url}
						alt="profile_photo"
						class="h-36"
						draggable="false"
						style="object-fit: cover;"
					/>
					<div class="p-4">
						<p class="text-md text-gray-600">
							{i.thought}	
						</p>
					</div>
				</Card>
			{/each}
		</div>
	</div>
</TimelineUtil>
