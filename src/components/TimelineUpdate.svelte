<script>
	import Card from './Card.svelte';
</script>

<!-- Timeline Container -->
<div class="flex flex-col md:flex-row md:justify-center">
	<div class="flex flex-col flex-shrink-0 items-center md:mr-8">
		<div class="text-gray-500 text-sm pt-24">Dec 2023</div>
	</div>
	<!-- <div class="py-4 flex items-center border-r-4 border-dotted relative mobile:h-72 max-mobile:h-36 mobile:w-40 ml-4 max-mobile:w-2 "> </div> -->
	<!-- Center Line -->
	<div class="relative md:flex border-r-4 border-dotted border-gray-300 mr-8">
		<div
			class="absolute top-24 left-1/2 -translate-x-1/2 flex justify-center items-center bg-blue-500 rounded-full w-5 h-5"
			style="margin-left: 1px;"
			>
			<div class="bg-white rounded-full w-3 h-3"></div>
		</div>
	</div>

	<div class=" flex flex-grow grid grid-cols-1 md:grid-cols-2 gap-8 m-4 mr-12 lg:mr-72">
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
