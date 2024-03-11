<script>
	import Button from "./Button.svelte";
	import Profile from "./Profile.svelte";

</script>


<header class="w-screen container mx-auto flex flex-col max-w-screen-2xl px-2 py-2 ">
	<div class="flex flex-row  px-5 ">
		<!-- Logo image -->
		<img src="assets/ic_duggup.svg" width="27px" height="27px" alt="Duggup Logo" />

		<!-- Page title -->
		<div class="font-semibold text-2xl ml-2 my-auto" style="color:#333333;">duggup</div>
        <div class="flex-grow "/>
        <div class=" lg:block hidden  my-auto">
			<div class="flex  flex-row">

			<a href="#" class="flex items-center text-blue-500 hover:text-blue-700 font-bold py-2 px-4">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					fill="none"
					viewBox="0 0 24 24"
					stroke-width="1.5"
					stroke="currentColor"
					class="w-6 h-6 mr-2"
				>
					<path
						stroke-linecap="round"
						stroke-linejoin="round"
						d="M2.25 12l8.954-8.955c.44-.439 1.152-.439 1.591 0L21.75 12M4.5 9.75v10.125c0 .621.504 1.125 1.125 1.125H9.75v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21h4.125c.621 0 1.125-.504 1.125-1.125V9.75M8.25 21h8.25"
					/>
				</svg>
				Home
			</a>

			<a href="#" class="flex items-center text-blue-500 hover:text-blue-700 font-bold py-2 px-4">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					fill="none"
					viewBox="0 0 24 24"
					stroke-width="1.5"
					stroke="currentColor"
					class="w-6 h-6 mr-2"
				>
					<path stroke-linecap="round" stroke-linejoin="round" d="M15.75 19.5L8.25 12l7.5-7.5" />
				</svg>
				Explore
			</a>

			<a href="#" class="flex items-center text-blue-500 hover:text-blue-700 font-bold py-2 px-4">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					fill="none"
					viewBox="0 0 24 24"
					stroke-width="1.5"
					stroke="currentColor"
					class="w-6 h-6 mr-2"
				>
					<path
						stroke-linecap="round"
						stroke-linejoin="round"
						d="M12 6.042A8.967 8.967 0 006 3.75c-1.052 0-2.062.18-3 .512v14.25A8.987 8.987 0 016 18c2.305 0 4.408.867 6 2.292m0-14.25a8.966 8.966 0 016-2.292c1.052 0 2.062.18 3 .512v14.25A8.987 8.987 0 0018 18a8.967 8.967 0 00-6 2.292m0-14.25v14.25"
					/>
				</svg>
				Learn
			</a>
			<Button text="Post" />
			<div class="m-4"/>
		</div>

		</div>
		<Profile/>
	</div>

	<!-- Horizontal dotted line -->
	<hr
		style="border-top: 1.5px dotted #525C69; border-top-style: dotted; border-top-width: 1.5px; border-top-color: #525C69; border-top-spacing: 3px;"
	/>
</header>
