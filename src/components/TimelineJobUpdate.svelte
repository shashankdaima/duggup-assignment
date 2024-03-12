<script lang="ts">
	import Card from './Card.svelte';
	import TimelineUtil from './TimelineUtil.svelte';
	export let job:any;

</script>

<!-- Timeline Container -->
<TimelineUtil>
	<div slot="timeline-left" class="my-auto flex-shrink-0 flex flex-col items-end ml-12 mr-6 mt-6">
		<img
		draggable="false"
			class="w-14 h-14 max-w-full max-h-full rounded-full"
			src={job.logo}
			alt="Chartr"
			style="border: 1px solid rgba(107, 114, 128, 0.5); border-radius: 50%;"
		/>
		<h6 class="self-end text-gray-900 font-semibold text-base text-right mt-2">{job.company_name}</h6>

		<p class="self-end text-gray-500 text-sm mt-1 text-right">{job.position}</p>
		<p class="self-end text-gray-500 text-sm mt-1 text-right">Joined on {job.join_date}</p>
	</div>

	<div slot="timeline-marker">
		
		<div
			class="absolute top-24 left-1/2 -translate-x-1/2 flex justify-center items-center bg-blue-500 rounded-full w-7 h-7"
			style="margin-left: 2px;"
		>
			<div class="bg-white rounded-full w-2 h-2"></div>
		</div>
		<div
			class="absolute  left-1/2 -translate-x-1/2 flex justify-center items-center w-7 h-4 "
			style="margin-left: 2px; background-color: #FCFCFF;"
		>
			<img draggable="false" src="assets/ic_arrow_up.svg"/>
		</div>
	
	</div>
	<div slot="body" class=" relative  gap-8 m-4 mt-8 p-4 lg:pr-64">
		<Card strokes={false}>
			<div class="p-5">
				<h6 class="text-xl font-bold" style="text-color: #141618;">
					{job.position}
				</h6>
				<p class="text-sm text-gray-400 mt-1">
					Full-time - Remote	
				</p>
			</div>
		</Card>
	</div>
</TimelineUtil>
