<script lang="ts">
	export let text: string;
</script>

<button
	class="my-auto pl-2 pr-4 py-1 bg-white border border-gray-400 rounded transition-all
        ease-in-out duration-150 focus:outline-none focus:ring-2 focus:ring-blue-300
        hover:shadow-lg transform active:shadow-none flex flex-row items-center"
	style="box-shadow: 0px 4px 0px 0px #4D4D4D;"
	on:mousedown={(e) => (e.currentTarget.style.boxShadow = '0px 0px 0px 0px #4D4D4D')}
	on:mouseup={(e) => (e.currentTarget.style.boxShadow = '0px 4px 0px 0px #4D4D4D')}
	on:mouseleave={(e) => (e.currentTarget.style.boxShadow = '0px 4px 0px 0px #4D4D4D')}
>
	<img class="mr-1" src="assets/ic_post.svg" width="27px" height="27px" alt="Dug" />
	<p class="text-m text-gray-600">{text}</p>
</button>
