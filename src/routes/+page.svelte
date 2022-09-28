<script>
	export let data
</script>

<div class="container mx-auto py-11">
	<div class="border-double border-4 border-grey-600 rounded-lg shadow-2xl bg-black/[0.5]">
		<div class="p-4">
			<div class="flex justify-center">
				<img src="https://picsum.photos/200/300" alt="" class="w-20 h-20 mr-10" />
				<div class="grid content-center">
					<span
						>Hello! I'm <strong>Erba Afidotama</strong>, and I'm web developer with full stack
						skill. I'm not pro, just still learning</span
					>
				</div>
			</div>
		</div>
	</div>

	<div class="flex flex-row">
		<div
			class="border-double border-4 border-grey-600 rounded-lg shadow-2xl mt-10 mr-4 basis-1/2 h-60 bg-black/[0.5]"
		>
			<div class="p-4">
				<ol class="relative border-l border-gray-200 dark:border-gray-700">
					<li class="mb-10 ml-4">
						<div
							class="absolute w-3 h-3 bg-gray-200 rounded-full mt-1.5 -left-1.5 border border-white dark:border-gray-900 dark:bg-gray-700"
						/>
						<time class="mb-1 text-sm font-normal leading-none text-gray-400 dark:text-gray-500"
							>September 2016 - July 2017</time
						>
						<h3 class="text-lg font-semibold text-white dark:text-white">
							Freelance Web Developer at Nokia
						</h3>
						<p class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400">
							Creating Nokia Website using CodeIgniter 3.
						</p>
					</li>
					<li class="mb-10 ml-4">
						<div
							class="absolute w-3 h-3 bg-gray-200 rounded-full mt-1.5 -left-1.5 border border-white dark:border-gray-900 dark:bg-gray-700"
						/>
						<time class="mb-1 text-sm font-normal leading-none text-gray-400 dark:text-gray-500"
							>November 2017 - Present</time
						>
						<h3 class="text-lg font-semibold text-white dark:text-white">
							Web Developer at PT.Trees Solutions
						</h3>
						<p class="text-base font-normal text-gray-500 dark:text-gray-400">
							Creating HR website using React as Frontend and Python as Backend.
						</p>
					</li>
				</ol>
			</div>
		</div>

		<div
			class="border-double border-4 border-grey-600 rounded-lg shadow-2xl mt-10 my-2 ml-4 basis-1/2 h-60 bg-black/[0.5]"
		>
			<div class="p-4">
				<div class="flex justify-center">
					<p class="text-4xl font-semibold">My Skill</p>
				</div>
				<div class="flex justify-center mt-5">
					<img src="/images/svelte-logo.png" alt="" class="w-18 h-20 mx-5" />
					<img src="/images/react-logo.png" alt="" class="w-18 h-20 mx-5" />
					<img src="/images/golang-logo.png" alt="" class="w-18 h-14 mx-5 mt-3" />
					<img src="/images/flutter-logo.png" alt="" class="w-18 h-20 mx-5" />
				</div>
			</div>
		</div>
	</div>

	<!-- BLOG -->
	<div class="mt-24">
		<p class="text-4xl text-white font-bold">My Blog</p>
	</div>
	<div class="grid grid-cols-4 gap-4 mt-5">
		{#each data.posts as post}
		<a
			href={post.path}
			class="block p-6 max-w-sm bg-white rounded-lg border border-gray-200 shadow-md hover:bg-gray-100 dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700"
		>
			<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
				{post.meta.title}
			</h5>
			<p class="font-normal text-gray-700 dark:text-gray-400">
				Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse
				chronological order.
			</p>
			<p class="mt-5">Published {post.meta.date}</p>
		</a>
	{/each}
	</div>

	<!-- GITHUB -->
	<div class="mt-24">
		<p class="text-4xl text-white font-bold">My Project</p>
	</div>
	<div class="grid grid-cols-4 gap-4 mt-5">
		<div
			class="block p-6 max-w-sm  rounded-lg border border-gray-200 shadow-md  bg-black/[0.5] hover:bg-black/[0.75] hover:border-double hover:border-4"
		>
			<div class="flex">
				<div class="w-14 h-14">
					<img src="/images/github.png" alt="" />
				</div>
				<h5
					class="mb-2 text-2xl font-bold tracking-tight self-center text-white-900 dark:text-white"
				>
					Klasemen
				</h5>
			</div>

			<p class="font-normal text-white-700 dark:text-gray-400">
				Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse
				chronological order.
			</p>
			<button
				class="block p-2 mt-2 max-w-sm  rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700 hover:bg-gray-800"
			>
				<div class="hover:text-white">Github</div>
			</button>
		</div>

		<div
			class="block p-6 max-w-sm  rounded-lg border border-gray-200 shadow-md bg-black/[0.5] hover:bg-black/[0.75] hover:border-double hover:border-4"
		>
			<div class="flex">
				<div class="w-14 h-14">
					<img src="/images/github.png" alt="" />
				</div>
				<h5
					class="mb-2 text-2xl font-bold tracking-tight self-center text-white-900 dark:text-white"
				>
					Klasemen
				</h5>
			</div>

			<p class="font-normal text-white-700 dark:text-gray-400">
				Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse
				chronological order.
			</p>
			<button
				class="block p-2 mt-2 max-w-sm  rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700 hover:bg-gray-800"
			>
				<div class="hover:text-white">Github</div>
			</button>
		</div>

		<div
			class="block p-6 max-w-sm  rounded-lg border border-gray-200 shadow-md bg-black/[0.5] hover:bg-black/[0.75] hover:border-double hover:border-4"
		>
			<div class="flex">
				<div class="w-14 h-14">
					<img src="/images/github.png" alt="" />
				</div>
				<h5
					class="mb-2 text-2xl font-bold tracking-tight self-center text-white-900 dark:text-white"
				>
					Klasemen
				</h5>
			</div>

			<p class="font-normal text-white-700 dark:text-gray-400">
				Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse
				chronological order.
			</p>
			<button
				class="block p-2 mt-2 max-w-sm  rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700 hover:bg-gray-800"
			>
				<div class="hover:text-white">Github</div>
			</button>
		</div>

		<div
			class="block p-6 max-w-sm  rounded-lg border border-gray-200 shadow-md bg-black/[0.5] hover:bg-black/[0.75] hover:border-double hover:border-4"
		>
			<div class="flex">
				<div class="w-14 h-14">
					<img src="/images/github.png" alt="" />
				</div>
				<h5
					class="mb-2 text-2xl font-bold tracking-tight self-center text-white-900 dark:text-white"
				>
					Klasemen
				</h5>
			</div>

			<p class="font-normal text-white-700 dark:text-gray-400">
				Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse
				chronological order.
			</p>
			<button
				class="block p-2 mt-2 max-w-sm  rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700 hover:bg-gray-800"
			>
				<div class="hover:text-white">Github</div>
			</button>
		</div>

		<div
			class="block p-6 max-w-sm  rounded-lg border border-gray-200 shadow-md bg-black/[0.5] hover:bg-black/[0.75] hover:border-double hover:border-4"
		>
			<div class="flex">
				<div class="w-14 h-14">
					<img src="/images/github.png" alt="" />
				</div>
				<h5
					class="mb-2 text-2xl font-bold tracking-tight self-center text-white-900 dark:text-white"
				>
					Klasemen
				</h5>
			</div>

			<p class="font-normal text-white-700 dark:text-gray-400">
				Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse
				chronological order.
			</p>
			<button
				class="block p-2 mt-2 max-w-sm  rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700 hover:bg-gray-800"
			>
				<div class="hover:text-white">Github</div>
			</button>
		</div>
	</div>
</div>

<!-- <style>
	:global(body) {
		/* background: linear-gradient(165deg, #1F7B61 0%, #fff 77%); */
		/* background-color: #f2eee2; */
		/* background-color: #31363b; */
		color: #ffffff;
		background-image: url('/images/cool-bg.png');
		background-repeat: repeat;
	}
</style> -->
