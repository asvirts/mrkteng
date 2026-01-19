<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import { title } from '$lib/index';

	let { children } = $props();

	let currentYear = $state(new Date().getFullYear());
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<title>{title}</title>
</svelte:head>

<header class="absolute inset-x-0 top-0 z-50 mx-auto max-w-7xl">
	<nav aria-label="Global" class="flex items-center justify-between p-6 lg:px-8">
		<div class="flex lg:flex-1">
			<a href="/" class="-m-1.5 p-1.5">
				<span class="sr-only">MrktEng</span>
				<img
					src="https://shy3m4o231.ufs.sh/f/McaFsfFI80o6KL6S6abMAODcG8FkHL9lpQIWZTuv1t3Y7Sq4"
					alt=""
					class="h-16 w-auto"
				/>
			</a>
		</div>
		<div class="flex lg:hidden">
			<button
				type="button"
				command="show-modal"
				commandfor="mobile-menu"
				class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-700"
			>
				<span class="sr-only">Open main menu</span>
				<svg
					viewBox="0 0 24 24"
					fill="none"
					stroke="currentColor"
					stroke-width="1.5"
					data-slot="icon"
					aria-hidden="true"
					class="size-6"
				>
					<path
						d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
						stroke-linecap="round"
						stroke-linejoin="round"
					/>
				</svg>
			</button>
		</div>
		<div class="hidden lg:flex lg:gap-x-12">
			<a href="/about" class="text-sm/6 font-semibold text-gray-900">About</a>
			<a href="/blog" class="text-sm/6 font-semibold text-gray-900">Blog</a>
			<a href="/tools" class="text-sm/6 font-semibold text-gray-900">Tools</a>
			<a href="/playbooks" class="text-sm/6 font-semibold text-gray-900">Playbooks</a>
		</div>
		<div class="hidden lg:flex lg:flex-1 lg:justify-end">
			<a href="/login" class="text-sm/6 font-semibold text-gray-900"
				>Log in <span aria-hidden="true">&rarr;</span></a
			>
		</div>
	</nav>
	<el-dialog>
		<dialog id="mobile-menu" class="backdrop:bg-transparent lg:hidden">
			<div class="fixed inset-0 focus:outline-none">
				<el-dialog-panel
					class="fixed inset-y-0 right-0 z-50 w-full overflow-y-auto bg-white p-6 sm:max-w-sm sm:ring-1 sm:ring-gray-900/10"
				>
					<div class="flex items-center justify-between">
						<a href="/" class="-m-1.5 p-1.5">
							<span class="sr-only">Your Company</span>
							<img
								src="https://tailwindcss.com/plus-assets/img/logos/mark.svg?color=indigo&shade=600"
								alt=""
								class="h-8 w-auto"
							/>
						</a>
						<button
							type="button"
							command="close"
							commandfor="mobile-menu"
							class="-m-2.5 rounded-md p-2.5 text-gray-700"
						>
							<span class="sr-only">Close menu</span>
							<svg
								viewBox="0 0 24 24"
								fill="none"
								stroke="currentColor"
								stroke-width="1.5"
								data-slot="icon"
								aria-hidden="true"
								class="size-6"
							>
								<path d="M6 18 18 6M6 6l12 12" stroke-linecap="round" stroke-linejoin="round" />
							</svg>
						</button>
					</div>
					<div class="mt-6 flow-root">
						<div class="-my-6 divide-y divide-gray-500/10">
							<div class="py-6">
								<a
									href="/about"
									class="-mx-3 block rounded-lg px-3 py-2 text-base/7 font-semibold text-gray-900 hover:bg-gray-50"
									>Company</a
								>
							</div>
							<div class="py-6">
								<a
									href="/login"
									class="-mx-3 block rounded-lg px-3 py-2.5 text-base/7 font-semibold text-gray-900 hover:bg-gray-50"
									>Log in</a
								>
							</div>
						</div>
					</div>
				</el-dialog-panel>
			</div>
		</dialog>
	</el-dialog>
</header>

{@render children()}

<footer class="bg-gray-100">
	<div class="relative mx-auto max-w-7xl px-4 py-16 sm:px-6 lg:px-8 lg:pt-24">
		<div class="absolute end-4 top-4 sm:end-6 sm:top-6 lg:end-8 lg:top-8">
			<a
				class="inline-block rounded-full bg-green-600 p-2 text-white shadow-sm transition hover:bg-green-500 sm:p-3 lg:p-4"
				href="#MainContent"
			>
				<span class="sr-only">Back to top</span>

				<svg
					xmlns="http://www.w3.org/2000/svg"
					class="size-5"
					viewBox="0 0 20 20"
					fill="currentColor"
				>
					<path
						fill-rule="evenodd"
						d="M14.707 12.707a1 1 0 01-1.414 0L10 9.414l-3.293 3.293a1 1 0 01-1.414-1.414l4-4a1 1 0 011.414 0l4 4a1 1 0 010 1.414z"
						clip-rule="evenodd"
					></path>
				</svg>
			</a>
		</div>

		<div class="lg:flex lg:items-end lg:justify-between">
			<div>
				<div class="flex justify-center text-green-600 lg:justify-start">
					<h2 class="text-4xl font-semibold tracking-tight text-balance text-green-600 transition">
						MrktEng
					</h2>
				</div>

				<p class="mx-auto mt-6 max-w-md text-center leading-relaxed text-gray-500 lg:text-left">
					Practical thinking on marketing systems, martech, and engineering tradeoffs — for people
					who actually have to make it work.
				</p>
			</div>

			<ul
				class="mt-12 flex flex-wrap justify-center gap-6 md:gap-8 lg:mt-0 lg:justify-end lg:gap-12"
			>
				<li>
					<a class="text-gray-700 transition hover:text-gray-700/75" href="/about"> About </a>
				</li>

				<li>
					<a class="text-gray-700 transition hover:text-gray-700/75" href="/blog"> Blog </a>
				</li>

				<li>
					<a class="text-gray-700 transition hover:text-gray-700/75" href="/tools"> Tools </a>
				</li>

				<li>
					<a class="text-gray-700 transition hover:text-gray-700/75" href="/playbooks">
						Playbooks
					</a>
				</li>
			</ul>
		</div>

		<p class="mt-12 text-center text-sm text-gray-500 lg:text-right">
			Copyright © {currentYear}. All rights reserved.
		</p>
	</div>
</footer>
