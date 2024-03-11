<script lang="ts">
	// Script block for any necessary JavaScript
</script>

<div class="flex w-full">
	<div class="flex-grow " style="max-width: 15%;">
        <slot name="timeline-left"></slot>
    </div>
	<div class="relative md:flex border-r-4 border-dotted border-gray-300">
        <slot name="timeline-marker"></slot>
    </div>
	<div  style="width: 84%;  padding: 10px;">
        <slot name="body"/>
    </div>
</div>


