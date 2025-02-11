<script>
	let isHovered = false;
	const text = 'supra-astra';
	const letters = text.split('');
</script>

<header class="sticky top-0 z-10 flex h-20 flex-col items-center gap-x-8">
	<h2
		class="p-4 text-2xl font-semibold"
		on:mouseenter={() => (isHovered = true)}
		on:mouseleave={() => (isHovered = false)}
	>
		<div class="flex">
			{#each letters as letter, i}
				<span
					class="inline-block transition-transform duration-300"
					class:animate-bounce={isHovered}
					style="animation-delay: {i * 50}ms"
				>
					{letter}
				</span>
			{/each}
		</div>
	</h2>
	<p class="w-1/2 text-center text-xl md:text-2xl">
		making game development easier and accessible with help of AI and modern systems programming!
	</p>
</header>

<style>
	.animate-bounce {
		animation: bounce 1s infinite;
	}

	@keyframes bounce {
		0%,
		100% {
			transform: translateY(0);
		}
		50% {
			transform: translateY(-10px);
		}
	}
</style>
