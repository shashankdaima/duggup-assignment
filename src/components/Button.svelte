<script lang="ts">
	export let text: string;
	export let icon: string | undefined = undefined;
</script>

<button
	class="my-auto px-4 py-1 bg-white border border-gray-400 rounded transition-all
        ease-in-out duration-150 transform active:shadow-none flex flex-row items-center"
	style="box-shadow: 0px 4px 0px 0px #4D4D4D;"
	on:mousedown={(e) => (e.currentTarget.style.boxShadow = '0px 0px 0px 0px #4D4D4D')}
	on:mouseup={(e) => (e.currentTarget.style.boxShadow = '0px 4px 0px 0px #4D4D4D')}
	on:mouseleave={(e) => (e.currentTarget.style.boxShadow = '0px 4px 0px 0px #4D4D4D')}
>

	{#if icon != undefined}
		<img class="mr-1" src={icon} width="27px" height="27px" alt="icon" />
	{/if}
	{#if icon != undefined}
		<p class="text-md text-gray-600 pr-3">{text}</p>
	{:else}
		<p class="text-md text-gray-600">{text}</p>
	{/if}
</button>
