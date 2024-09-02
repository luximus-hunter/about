<script lang="ts">
	import * as Avatar from '$lib/components/ui/avatar';
	import { Button } from '$lib/components/ui/button';
	import Discord from '$lib/components/ui/icons/discord.svelte';
	import Github from '$lib/components/ui/icons/github.svelte';
	import LinkedIn from '$lib/components/ui/icons/linkedin.svelte';
	import Spotify from '$lib/components/ui/icons/spotify.svelte';
	import * as Card from '$lib/components/ui/card';
</script>

<div class="grid h-dvh w-full grid-cols-1 place-items-center p-4">
	<main>
		<Card.Root>
			<Card.Content class="flex gap-4 p-4">
				<Avatar.Root class="row-span-2 h-32 w-32">
					<Avatar.Image src="/profile-picture.png" alt="Luximus" class="bg-white" />
					<Avatar.Fallback>LUX</Avatar.Fallback>
				</Avatar.Root>
				<div class="flex flex-1 flex-col align-middle">
					<h1 class="scroll-m-20 text-4xl font-extrabold tracking-tight lg:text-5xl">
						Thomas Lipman
					</h1>
					<p class="text-2xl text-muted-foreground lg:text-4xl">Luximus</p>
					<p class="text-sm text-muted-foreground">Student at Windesheim University</p>
					<p class="text-sm text-muted-foreground">Junior Web Dev</p>
				</div>
			</Card.Content>
		</Card.Root>
		<section class="mt-4 grid grid-cols-1 gap-4 sm:grid-cols-2 md:grid-cols-4">
			<Button
				size="lg"
				variant="outline"
				href="https://github.com/luximus-hunter"
				class="hover:border-[#24292e] hover:bg-[#2d333b] hover:text-white dark:hover:border-[#dddddd] dark:hover:bg-[#ffffff] dark:hover:text-black"
			>
				<Github class="mr-2 h-6 w-6" /> Github
			</Button>
			<Button
				size="lg"
				variant="outline"
				href="https://www.linkedin.com/in/thomas-lipman/"
				class="hover:border-[#084d91] hover:bg-[#0A66C2] hover:text-white"
			>
				<LinkedIn class="mr-2 h-6 w-6" />LinkedIn
			</Button>
			<Button
				size="lg"
				variant="outline"
				href="https://discordapp.com/users/306692821358739456"
				class="hover:border-[#2a3aef] hover:bg-[#5865F2] hover:text-white"
			>
				<Discord class="mr-2 h-6 w-6" />Discord
			</Button>
			<Button
				size="lg"
				variant="outline"
				href="https://open.spotify.com/user/yxmq93tlmfomm2ir62cs0bq0u"
				class="hover:border-[#189a46] hover:bg-[#1DB954] hover:text-white"
			>
				<Spotify class="mr-2 h-6 w-6" />Spotify
			</Button>
		</section>
	</main>
</div>
