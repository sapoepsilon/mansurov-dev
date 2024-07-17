<script lang="ts">
	import { cn } from "$lib/utils";
	import BlogCard from "$lib/components/BlogCard.svelte";

	const blogPosts = [
		{
			title: "Blog post heading",
			body: "Blog body text lorem ipsum lorem ipsum lorem ipsu",
			imageUrl: "https://picsum.photos/536/354"
		},
		{
			title: "Blog post heading",
			body: "Body text for whatever you'd like to say. Add main takeaway points, quotes, anecdotes, or even a very very short story.",
			imageUrl: "https://picsum.photos/536/355"
		},
		{
			title: "Title",
			body: "Body text for whatever you'd like to say. Add main takeaway points, quotes, anecdotes, or even a very very short story.",
			imageUrl: "https://picsum.photos/536/356"
		}
	];
</script>

<section class={cn("flex flex-col items-start justify-start min-h-[calc(100vh-48px)] bg-background text-foreground p-4 md:p-8")}>
	<div class="lg:ml-36 md:ml-24">
	<h1 class="text-4xl md:text-6xl font-bold mb-2">Blog</h1>
	<p class="text-xl md:text-2xl text-muted-foreground mb-8">My thoughts</p>
	</div>
	<div class="w-full space-y-4 flex flex-col items-center">
		{#each blogPosts as post}
			<BlogCard
				title={post.title}
				body={post.body}
				imageUrl={post.imageUrl}
			/>
		{/each}
	</div>
</section>
