<script lang="ts">
	import moodle_logo from '$lib/assets/moodle_logo.ico';
	import pdf_logo from '$lib/assets/pdf_logo.png';
</script>

<svelte:head>
	<title>Lecture 1: Introduction to Software Development and Design</title>
	<meta name="description" content="Lecture 1 covers the fundamentals of Software Development and Design, including Coupling, Cohesion, DRY principles, SOLID principles, and design patterns." />
	<meta name="keywords" content="Software Development, Software Design, Coupling, Cohesion, DRY Principles, SOLID Principles, Design Patterns, Lecture 1" />
	<meta name="author" content="Samuel" />
	<meta name="language" content="en-UK" />
</svelte:head>

<main class="relative flex h-screen flex-1 flex-col overflow-hidden bg-slate-50">
	<header class="sticky top-0 z-20 border-b border-slate-200 bg-white shadow-sm">
		<div class="flex items-center justify-between px-8 py-4">
			<div>
				<h1 class="text-2xl font-bold text-slate-800">Lecture 1: Introduction to Software Development and Design</h1>
			</div>
			<nav class="hidden space-x-4 text-sm font-medium text-slate-600 md:flex">
				<a href="#overview" class="transition-colors hover:text-indigo-600">Overview</a>
				<a href="#pdf-viewer" class="transition-colors hover:text-indigo-600">Lecture PDF</a>
				<a href="#key-concepts" class="transition-colors hover:text-indigo-600">Key Concepts</a>
				<a href="#resources" class="transition-colors hover:text-indigo-600">Resources</a>
			</nav>
		</div>
	</header>

	<div class="flex-1 overflow-y-auto p-8">
		<div class="mx-auto max-w-4xl space-y-12 pb-20">
			<section id="overview" class="space-y-4">
				<h2 class="border-l-4 border-indigo-500 pl-3 text-xl font-bold text-slate-800">Overview</h2>
				<p class="leading-relaxed text-slate-600">
					This lecture introduces the fundamentals of Software Development and Design, covering the Coupling, Cohesion, DRY principles, SOLID principles, and various design patterns. Understanding
					these concepts is crucial for creating maintainable and efficient software systems.
				</p>
				<div class="rounded-lg border border-blue-200 bg-blue-50 p-4 text-sm text-blue-800">
					<strong>Exam Tip:</strong> Focus on understanding the principles of Coupling and Cohesion, as well as the DRY principle.
				</div>
			</section>

			<hr class="border-slate-200" />

			<section id="pdf-viewer" class="space-y-4">
				<h2 class="border-l-4 border-indigo-500 pl-3 text-xl font-bold text-slate-800">Lecture Material (PDF)</h2>

				<div class="flex h-96 w-full flex-col items-center justify-center rounded-lg border-2 border-dashed border-slate-400 bg-slate-200 text-slate-500">
					<!-- <svg class="mb-2 h-12 w-12 opacity-50" fill="none" viewBox="0 0 24 24" stroke="currentColor">
						<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 21h10a2 2 0 002-2V9.414a1 1 0 00-.293-.707l-5.414-5.414A1 1 0 0012.586 3H7a2 2 0 00-2 2v14a2 2 0 002 2z" />
					</svg>
					<p class="font-medium">Embed PDF Here</p>
					<p class="mt-1 text-xs text-slate-400">&lt;iframe src="lecture1.pdf" class="w-full h-full"&gt;&lt;/iframe&gt;</p> -->
					<iframe title="Week 1 PDF" src="/assets/lecture1.pdf" class="h-full w-full"></iframe>
				</div>
				<div class="flex gap-3">
					<a href="/assets/lecture1.pdf" download class="rounded-md bg-indigo-600 px-4 py-2 text-sm text-white hover:bg-indigo-700">Download PDF</a>
					<a href="/assets/lecture1.pdf" target="_blank" rel="noopener noreferrer" class="rounded-md border border-slate-300 bg-white px-4 py-2 text-sm text-slate-700 hover:bg-slate-50"
						>Open in New Tab</a
					>
				</div>
			</section>

			<hr class="border-slate-200" />

			<section id="key-concepts" class="space-y-4">
				<h2 class="border-l-4 border-indigo-500 pl-3 text-xl font-bold text-slate-800">Key Concepts & Notes</h2>
				<ul class="grid grid-cols-1 gap-4 md:grid-cols-2">
					<li class="rounded border border-slate-200 bg-white p-4 shadow-sm">
						<h3 class="font-bold text-indigo-600">Coupling</h3>
						<p class="mt-1 text-sm text-slate-600">Degree of interdependence between software modules.</p>
					</li>
					<li class="rounded border border-slate-200 bg-white p-4 shadow-sm">
						<h3 class="font-bold text-indigo-600">Cohesion</h3>
						<p class="mt-1 text-sm text-slate-600">Degree to which the elements of a module belong together.</p>
					</li>
					<li class="rounded border border-slate-200 bg-white p-4 shadow-sm">
						<h3 class="font-bold text-indigo-600">DRY Principles</h3>
						<p class="mt-1 text-sm text-slate-600">Don't Repeat Yourself - a principle aimed at reducing repetition of software patterns.</p>
					</li>
					<li class="rounded border border-slate-200 bg-white p-4 shadow-sm">
						<h3 class="font-bold text-indigo-600">SOLID Principles</h3>
						<p class="mt-1 text-sm text-slate-600">A set of design principles for object-oriented programming to create more maintainable software.</p>
					</li>
				</ul>
			</section>

			<hr class="border-slate-200" />

			<section id="resources" class="space-y-4">
				<h2 class="border-l-4 border-indigo-500 pl-3 text-xl font-bold text-slate-800">Tools & Further Reading</h2>
				<div class="divide-y divide-slate-200 rounded-lg border border-slate-200 bg-white">
					<div class="flex items-center justify-between p-4 hover:bg-slate-50">
						<div class="flex items-center gap-3">
							<div class="flex h-8 w-8 items-center justify-center rounded text-xs font-bold">
								<img src={moodle_logo} alt="Moodle Logo" class="h-6 w-6" />
							</div>
							<div>
								<p class="text-sm font-medium text-slate-900">VLE Page</p>
								<p class="text-xs text-slate-500">Course management and resources.</p>
							</div>
						</div>
						<a target="_blank" href="https://learn.gold.ac.uk/course/section.php?id=569323" class="text-sm text-indigo-600 hover:underline">Link</a>
					</div>
					<div class="flex items-center justify-between p-4 hover:bg-slate-50">
						<div class="flex items-center gap-3">
							<div class="flex h-8 w-8 items-center justify-center rounded text-xs font-bold">
								<img src={pdf_logo} alt="PDF Logo" class="h-6 w-6" />
							</div>
							<div>
								<p class="text-sm font-medium text-slate-900">Design Principles and Design Patterns</p>
								<p class="text-xs text-slate-500">Additional reading on software design.</p>
							</div>
						</div>
						<a target="_blank" href="https://staff.cs.utu.fi/~jounsmed/doos_06/material/DesignPrinciplesAndPatterns.pdf" class="text-sm text-indigo-600 hover:underline">Link</a>
					</div>
					<div class="flex items-center justify-between p-4 hover:bg-slate-50">
						<div class="flex items-center gap-3">
							<div class="flex h-8 w-8 items-center justify-center rounded text-xs font-bold">
								<img src={pdf_logo} alt="PDF Logo" class="h-6 w-6" />
							</div>
							<div>
								<p class="text-sm font-medium text-slate-900">Coupling and Cohesion Metrics</p>
								<p class="text-xs text-slate-500">Research paper on measuring coupling and cohesion.</p>
							</div>
						</div>
						<a target="_blank" href="https://dl.acm.org/doi/10.1145/3172871.3172878" class="text-sm text-indigo-600 hover:underline">Link</a>
					</div>
				</div>
			</section>
		</div>
	</div>
</main>
