<script lang="ts">
	import Button from './Button.svelte';
	export let name: string;
	export let role: string;
	export let company: string;
	export let bio: string;
	export let companyLogo: string;
	export let profileImage: string;
</script>

<div class="flex flex-col lg:flex-row py-12 justify-center items-center">
	<div class="flex-shrink-0 flex flex-col justify-center max-w-36">
		<img
			class="h-32 w-32 rounded-full mx-auto"
			style="border: 5px solid #EAEFF5; border-radius: 50%;"
			src={profileImage}
			alt={name}
		/>
		<p class="font-semibold text-2xl text-center mt-3 text-gray-600 leading-tight">{name}</p>
	</div>

	<div class="flex flex-col justify-center lg:ml-8 max-w-lg lg:max-w-max">
		<p class="text-gray-600 about-me text-center lg:text-left">{role} at {company} {bio}</p>
		<div
			class="flex flex-col justify-center items-center mt-2 lg:mt-6 lg:block lg:justify-start lg:items-start"
		>
			<Button text="Follow" />
		</div>
	</div>
	<div class="my-auto flex-shrink-0 flex flex-col items-end ml-12 mr-8 lg:mr-0 hidden lg:block">
		<img
			draggable="false"
			class="h-14 rounded-full"
			src={companyLogo}
			alt={company}
			style="border: 1px solid rgba(107, 114, 128, 0.5); border-radius: 50%;"
		/>
		<h6 class="self-end text-gray-900 font-semibold text-base mt-2">
			{company}
		</h6>

		<p class="self-end text-gray-500 text-sm mt-1">
			{role}
		</p>
		<div class="flex flex-row mt-2 items-center">
			<p class="self-end text-gray-900 text-base mt-2 my-auto">My website</p>

			<img src="assets/ic_link_external.svg" class="h-4 w-4 ml-2 mt-2" alt="link" />

			<img src="assets/ic_menu_horizontal.svg" class="h-6 w-6 ml-2 mt-1" alt="menu" />
		</div>
	</div>
</div>

<style>
	/* You can add additional styles here if needed */
	.about-me {
		font-size: 17px;
		font-weight: 400;
		line-height: 28px;
		letter-spacing: 0em;
		color: #141618;
	}
</style>
