<script lang="ts">
	import '../app.css';

	let { children } = $props();
</script>

<div class="min-h-screen bg-neutral-900 text-neutral-200">
	{@render children()}
</div>
