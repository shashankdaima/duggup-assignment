<script>
	import Button from './Button.svelte';
	export let name = 'Shashank Daima';
	export let role = 'Co-Founder and CEO';
	export let company = 'Duggup';
	export let bio =
		'Social network for people in tech. Ex-Amazon Head of Engineering. I write hot-takes on building a business, shipping delightful products and accelerating product and career growth.';
</script>

<div class="flex flex-row py-12">
	<div class="flex-shrink-0 flex flex-col justify-center max-w-36">
		<img class="h-32 w-32 rounded-full  mx-auto" style="border: 5px solid #EAEFF5; border-radius: 50%;" src="assets/profile_photo.png" alt={name} />
		<p class="font-semibold text-2xl text-center mt-3 text-gray-600 leading-tight">{name}</p>
	</div>

	<div class="flex flex-col justify-center ml-8">
		<p class="text-gray-600 about-me">{role} at {company} {bio}</p>
		<div class="mt-6">
			<Button text="Follow" />
		</div>
	</div>
	<div class="my-auto flex-shrink-0 flex flex-col items-end ml-12 mr-8 lg:mr-0">
		<img
			class="h-14 rounded-full"
			src="https://play-lh.googleusercontent.com/RLYbkW34nzdwyj_S1QX8rcwAl6BPdlOliZRmk2h_zBlhH8L2aNODh64s1uV8ZGe14g=w240-h480-rw"
			alt="Chartr"
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

			<img src="assets/ic_menu_horizontal.svg" class="h-6 w-6 ml-2 mt-1 " alt="menu" />
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
		text-align: left;
		color: #141618;
	}
</style>
