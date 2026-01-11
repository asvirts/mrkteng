<script>
	let title = $state('Marketing, built like software.');

	function changeTitle() {
		title =
			title === 'Marketing, built like software.'
				? 'Software, built by marketing.'
				: 'Marketing, built like software.';
	}

	$effect(() => {
		const interval = setInterval(changeTitle, 3000);
		return () => clearInterval(interval);
	});
</script>

<div class="bg-white">
	<div class="relative isolate px-6 pt-14 lg:px-8">
		<div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-56">
			<div class="hidden sm:mb-8 sm:flex sm:justify-center">
				<div
					class="relative rounded-full px-3 py-1 text-sm/6 text-gray-600 ring-1 ring-gray-900/10 hover:ring-gray-900/20"
				>
					Marketing x Engineering. <a href="#" class="font-semibold text-green-600"
						><span aria-hidden="true" class="absolute inset-0"></span>Read more
						<span aria-hidden="true">&rarr;</span></a
					>
				</div>
			</div>
			<div class="text-center">
				<h1
					class="text-5xl font-semibold tracking-tight text-balance text-gray-900 transition sm:text-7xl"
				>
					{title}
				</h1>
				<p class="mt-8 text-lg font-medium text-pretty text-gray-500 sm:text-xl/8">
					Practical thinking on marketing systems, martech, and engineering tradeoffs — for people
					who actually have to make it work.
				</p>
				<div class="mt-10 flex items-center justify-center gap-x-6">
					<a
						href="#"
						class="rounded-md bg-green-600 px-3.5 py-2.5 text-sm font-semibold text-white shadow-xs transition-colors hover:bg-green-700 focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-green-600"
						>Get started</a
					>
					<a href="#" class="text-sm/6 font-semibold text-gray-900"
						>Learn more <span aria-hidden="true">→</span></a
					>
				</div>
			</div>
		</div>
	</div>
</div>

<div class="overflow-hidden bg-white py-24 sm:py-32">
	<div class="mx-auto max-w-7xl px-6 lg:px-8">
		<div
			class="mx-auto grid max-w-2xl grid-cols-1 gap-x-8 gap-y-16 sm:gap-y-20 lg:mx-0 lg:max-w-none lg:grid-cols-2"
		>
			<div class="lg:pt-4 lg:pr-8">
				<div class="lg:max-w-lg">
					<h2 class="text-base/7 font-semibold text-green-600">Build better systems</h2>
					<p
						class="mt-2 text-4xl font-semibold tracking-tight text-pretty text-gray-900 sm:text-5xl"
					>
						Stop asking product engineers to fix marketing.
					</p>
					<p class="mt-6 text-lg/8 text-gray-700">
						Marketing problems don’t disappear when you ignore them — they get pushed onto whoever
						can write code.
					</p>
					<dl class="mt-10 max-w-xl space-y-8 text-base/7 text-gray-600 lg:max-w-none">
						<div class="relative pl-9">
							<dt class="inline font-semibold text-gray-900">
								<svg
									viewBox="0 0 20 20"
									fill="currentColor"
									data-slot="icon"
									aria-hidden="true"
									class="absolute top-1 left-1 size-5 text-green-600"
								>
									<path
										d="M5.5 17a4.5 4.5 0 0 1-1.44-8.765 4.5 4.5 0 0 1 8.302-3.046 3.5 3.5 0 0 1 4.504 4.272A4 4 0 0 1 15 17H5.5Zm3.75-2.75a.75.75 0 0 0 1.5 0V9.66l1.95 2.1a.75.75 0 1 0 1.1-1.02l-3.25-3.5a.75.75 0 0 0-1.1 0l-3.25 3.5a.75.75 0 1 0 1.1 1.02l1.95-2.1v4.59Z"
										clip-rule="evenodd"
										fill-rule="evenodd"
									/>
								</svg>
								Protect product velocity.
							</dt>
							<dd class="inline">
								Product engineers stay focused on user-facing features instead of campaign plumbing.
							</dd>
						</div>
						<div class="relative pl-9">
							<dt class="inline font-semibold text-gray-900">
								<svg
									viewBox="0 0 20 20"
									fill="currentColor"
									data-slot="icon"
									aria-hidden="true"
									class="absolute top-1 left-1 size-5 text-green-600"
								>
									<path
										d="M10 1a4.5 4.5 0 0 0-4.5 4.5V9H5a2 2 0 0 0-2 2v6a2 2 0 0 0 2 2h10a2 2 0 0 0 2-2v-6a2 2 0 0 0-2-2h-.5V5.5A4.5 4.5 0 0 0 10 1Zm3 8V5.5a3 3 0 1 0-6 0V9h6Z"
										clip-rule="evenodd"
										fill-rule="evenodd"
									/>
								</svg>
								Own marketing’s technical surface area.
							</dt>
							<dd class="inline">
								Integrations, automation, data contracts, experimentation, and tooling live with a
								team designed to maintain them.
							</dd>
						</div>
						<div class="relative pl-9">
							<dt class="inline font-semibold text-gray-900">
								<svg
									viewBox="0 0 20 20"
									fill="currentColor"
									data-slot="icon"
									aria-hidden="true"
									class="absolute top-1 left-1 size-5 text-green-600"
								>
									<path
										d="M4.632 3.533A2 2 0 0 1 6.577 2h6.846a2 2 0 0 1 1.945 1.533l1.976 8.234A3.489 3.489 0 0 0 16 11.5H4c-.476 0-.93.095-1.344.267l1.976-8.234Z"
									/>
									<path
										d="M4 13a2 2 0 1 0 0 4h12a2 2 0 1 0 0-4H4Zm11.24 2a.75.75 0 0 1 .75-.75H16a.75.75 0 0 1 .75.75v.01a.75.75 0 0 1-.75.75h-.01a.75.75 0 0 1-.75-.75V15Zm-2.25-.75a.75.75 0 0 0-.75.75v.01c0 .414.336.75.75.75H13a.75.75 0 0 0 .75-.75V15a.75.75 0 0 0-.75-.75h-.01Z"
										clip-rule="evenodd"
										fill-rule="evenodd"
									/>
								</svg>
								Turn growth into software.
							</dt>
							<dd class="inline">
								Repeatable, testable systems instead of spreadsheets, Zapier chains, and hope.
							</dd>
						</div>
					</dl>
				</div>
			</div>
			<img
				width="2432"
				height="1442"
				src="https://images.unsplash.com/photo-1553877522-43269d4ea984?q=80&w=1740&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
				alt="Product screenshot"
				class="w-3xl max-w-none rounded-xl shadow-xl ring-1 ring-gray-400/10 sm:w-228 md:-ml-4 lg:-ml-0"
			/>
		</div>
	</div>
</div>
