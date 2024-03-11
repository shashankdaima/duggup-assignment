<script>
	import Card from './Card.svelte';
	import TimelineUtil from './TimelineUtil.svelte';
</script>

<!-- Timeline Container -->
<TimelineUtil>
	<div slot="timeline-left">
		<p class="text-gray-500 text-sm text-right mt-24 mr-4">Dec 2023</p>
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
		<div  class="grid grid-cols-1 md:grid-cols-2 gap-8 m-4 mr-12 ml-8 lg:mr-72">
			<Card strokes={true}>
				<img
					src="assets/profile_photo.png"
					alt="profile_photo"
					class="h-36"
					draggable="false"
					style="object-fit: cover;"
				/>
				<div class="p-4">
					<p class="text-md text-gray-600">
						World can be better place if linkedin users don't ghost each other.
					</p>
				</div>
			</Card>
			<Card strokes={true}>
				<img
					src="assets/profile_photo.png"
					alt="profile_photo"
					class="h-36"
					style="object-fit: cover;"
				/>
				<div class="p-4">
					<p class="text-md text-gray-600">
						World can be better place if linkedin users don't ghost each other.
					</p>
				</div>
			</Card>
			<Card strokes={true}>
				<img
					src="assets/profile_photo.png"
					alt="profile_photo"
					class="h-36"
					style="object-fit: cover;"
				/>
				<div class="p-4">
					<p class="text-md text-gray-600">
						World can be better place if linkedin users don't ghost each other.
					</p>
				</div>
			</Card>
		</div>
	</div>
</TimelineUtil>