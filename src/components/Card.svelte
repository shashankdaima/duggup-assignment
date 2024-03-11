<script lang="ts">
	export let strokes:boolean=false;
</script>
<div
	class="flex flex-col bg-white rounded-lg w-full shadow-sm overflow-hidden {!strokes
		? ''
		: 'border border-gray-300'} "
>
	<slot />
</div>
