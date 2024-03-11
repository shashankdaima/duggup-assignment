<script>
	import Card from './Card.svelte';
</script>

<!-- Timeline Container -->
<div class="flex flex-col md:flex-row md:justify-center ">
	<div class="flex flex-col flex-shrink-0 items-center md:mr-8">
		<div class="text-gray-500 text-sm pt-14">Dec 2023</div>
	</div>

	<!-- Center Line -->
	<div class="relative md:flex border-r-2 border-gray-300 mr-8">
		<div
			class="absolute top-12 left-1/2 -translate-x-1/2 flex justify-center items-center bg-blue-500 rounded-full w-8 h-8"
			style="margin-left: 1px;" 
			>
			<div class="bg-white rounded-full w-3 h-3"></div>
		</div>
	</div>

	<div class=" flex flex-grow grid grid-cols-1 gap-8 m-4 mr-12 lg:mr-72">
		<Card>
			<div class="p-4">

				<h3 class="text-left text-2xl font-bold leading-8 tracking-normal">
					Co-Founder and CEO
				</h3>
				<p class="text-sm text-gray-600 mt-1 ">Full-time · Remote</p>
			</div>
		</Card>
	</div>
</div>
