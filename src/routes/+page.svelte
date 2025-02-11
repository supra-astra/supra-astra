<script lang="ts">
	import Footer from '$lib/components/footer.svelte';
	import Header from '$lib/components/header.svelte';
</script>

<div class="flex h-screen flex-col items-center justify-center p-4">
	<Header />
	<div class="flex h-screen flex-col items-center justify-center gap-y-6 p-4">
		<a href="/about">about</a>
		<a href="/blog">research</a>
	</div>
	<Footer />
</div>
