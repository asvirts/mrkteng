<script>
	let title = $state('Log in');
</script>

<div class="bg-white">
	<div class="relative isolate px-6 pt-14 lg:px-8">
		<div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-56">
			<div class="text-center">
				<h1
					class="text-7xl font-semibold tracking-tight text-balance text-gray-900 transition sm:text-7xl"
				>
					{title}
				</h1>
				<p class="mt-8 text-lg font-medium text-pretty text-gray-500 sm:text-xl/8">
					Access your MrktEng account.
				</p>
				<div class="mt-10 flex items-center justify-center gap-x-6">
					<button
						class="rounded-md bg-green-600 px-3.5 py-2.5 text-sm font-semibold text-white shadow-xs transition-colors hover:bg-green-700 focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-green-600"
					>
						Sign in
					</button>
					<a href="/" class="text-sm/6 font-semibold text-gray-900">
						Back to home <span aria-hidden="true">→</span>
					</a>
				</div>
			</div>
		</div>
	</div>
</div>
