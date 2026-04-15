<script lang="ts">
	let { title, cols } = $props();
</script>

<div class="{cols} row-span-1 h-full w-full rounded-2xl bg-base-200">
	<div class="flex h-full flex-row items-center justify-center">
		<h1 class="text-center font-[Space_Grotesk_Variable] text-4xl font-bold text-base-content">
			{title}
		</h1>
	</div>
</div>
