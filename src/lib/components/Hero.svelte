<script lang="ts">
	import { cn } from "$lib/utils";
	let headline = "Ismatulla Mansurov";
	let subheadline = "I automate things";
</script>

<section class={cn("flex flex-col items-center justify-center min-h-[calc(100vh-48px)] bg-background text-foreground")}>
	<h1 class="text-8xl font-bold mb-4 text-center">{headline}</h1>
	<p class="text-2xl text-muted-foreground">{subheadline}</p>
</section>
