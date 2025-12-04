---
layout: default
title: News
---
<!-- Include Tailwind CSS CDN for local preview and robust styling -->
<script src="https://cdn.tailwindcss.com"></script>
<style>
    /* Ensure the body uses Inter font, common for academic sites */
    body {
        font-family: 'Inter', sans-serif;
    }
</style>

<div class="container mx-auto px-4 py-8">
    <h1 class="text-4xl font-extrabold text-center text-gray-800 mt-8 mb-4">News & Updates</h1>
    <hr class="my-8 border-gray-300 w-24 mx-auto">

    <!-- Content Wrapper: max-width-3xl (approx 640px) is clean for reading -->
    <div class="max-w-3xl mx-auto">

        <!-- NEWS BLOCK START: Latest News -->
        <div class="flex flex-col md:flex-row items-start mb-10 pb-6 border-b border-gray-200">

            <!-- Text Content -->
            <div class="flex-1 pr-0 md:pr-8 order-2 md:order-1">
                <h2 class="text-2xl font-semibold text-indigo-700 mb-2 hover:text-indigo-900 transition-colors">
                    New Publication: 2D Materials for Memristors
                </h2>

                <p class="text-gray-700 leading-relaxed mb-3">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore
                    et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
                    aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
                    cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
                    culpa qui officia deserunt mollit anim id est laborum.
                </p>
                <a href="#" class="text-sm font-medium text-indigo-500 hover:text-indigo-700">Read More →</a>

                <!-- Meta Information -->
                <p class="text-xs text-gray-500 mt-2">
                    Andrea Capasso — January 14, 2025
                </p>
            </div>

            <!-- Image Container -->
            <div class="w-full md:w-36 h-36 overflow-hidden flex-shrink-0 rounded-lg shadow-md mb-4 md:mb-0 order-1 md:order-2">
                <img src="/assets/news/example.jpg"
                     alt="Placeholder image for news story"
                     class="w-full h-full object-cover transition-transform duration-300 hover:scale-105"
                     onerror="this.onerror=null; this.src='https://placehold.co/150x150/e0e7ff/4338ca?text=RESEARCH';"
                >
            </div>

        </div>
        <!-- NEWS BLOCK END -->


        <!-- NEWS BLOCK START: Older Item -->
        <div class="flex flex-col md:flex-row items-start mb-10 pb-6 border-b border-gray-200">

            <!-- Text Content -->
            <div class="flex-1 pr-0 md:pr-8 order-2 md:order-1">
                <h2 class="text-2xl font-semibold text-gray-700 mb-2 hover:text-gray-900 transition-colors">
                    Grant Awarded for Space Exploration Research
                </h2>

                <p class="text-gray-700 leading-relaxed mb-3">
                    Older news item: We are thrilled to announce that our lab has been awarded the prestigious SpaceTech
                    grant to develop novel sensing technologies for deep space missions. This project will run for four
                    years and involves collaboration with two international universities.
                </p>
                <a href="#" class="text-sm font-medium text-indigo-500 hover:text-indigo-700">View Details →</a>


                <!-- Meta Information -->
                <p class="text-xs text-gray-500 mt-2">
                    Andrea Capasso — March 2, 2019
                </p>
            </div>

            <!-- Image Container -->
            <div class="w-full md:w-36 h-36 overflow-hidden flex-shrink-0 rounded-lg shadow-md mb-4 md:mb-0 order-1 md:order-2">
                <img src="/assets/news/another.jpg"
                     alt="Placeholder image for older news story"
                     class="w-full h-full object-cover transition-transform duration-300 hover:scale-105"
                     onerror="this.onerror=null; this.src='https://placehold.co/150x150/d1d5db/374151?text=GRANT';"
                >
            </div>

        </div>
        <!-- NEWS BLOCK END -->

        <!-- You can paste the block above to add more news items -->

    </div>
</div>
