---
layout: new-layouts/base
title: Welcome to Swift.org
label: homepage
atom: true
---

{% capture code-snippet %}
    {% assign random_snippet = site.data.featured_snippets | sample %}
    {% include new-includes/components/box.html
        type="code"
        language="swift"
        content=random_snippet
        css="overflow-x:scroll"
    %}
{% endcapture %}
{% capture claim-section %}
<div class="grid-2-cols grid grid-cols-1 md:grid-cols-2 gap-16 items-center">
    <div class="claim space-y-8">
        <span class="inline-flex items-center rounded-full px-4 py-1 text-xs font-medium bg-orange-100 text-orange-800 dark:bg-orange-900/20 dark:text-orange-300">Swift 6 Is Here</span>
        <h1 class="text-5xl md:text-5xl font-bold text-gray-900 dark:text-white leading-tight">
            Fast, modern, safe, and a joy to write.
        </h1>
        <p class="text text-xl text-gray-600 dark:text-gray-300 max-w-xl" markdown=1>
            Swift is a general-purpose programming language that's approachable for newcomers and powerful for experts.
        </p>

        <div class="flex flex-col sm:flex-row gap-4 pt-2">
            <a href="/getting-started/" class="inline-flex items-center px-4 py-2 border border-transparent text-sm font-medium rounded-md text-white bg-orange-600 hover:bg-orange-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-orange-500 shadow-sm transition-all">
                Get Started
            </a>
            <a href="/about/" class="inline-flex items-center px-4 py-2 border border-gray-300 dark:border-gray-700 shadow-sm text-sm font-medium rounded-md text-gray-700 dark:text-gray-300 bg-white dark:bg-gray-800 hover:bg-gray-50 dark:hover:bg-gray-700 transition-colors">
                Learn More
            </a>
        </div>
    </div>
    <div class="max-w-lg mx-auto md:mx-0 rounded-2xl shadow-xl overflow-hidden bg-gray-900">
        {{ code-snippet }}
    </div>
</div>
{% endcapture %}
{% include new-includes/components/section.html
    content=claim-section
    css="py-24 md:py-36"
%}

{% capture banner-section %}
<div class="grid-1-cols">
    {% include new-includes/components/banner.html
        style="purple"
        text="Get ready for the Swift 6 language mode with the <a href=\"https://www.swift.org/migration/documentation/migrationguide\" class=\"font-semibold underline hover:text-purple-100 transition-colors\">official migration guide</a>"
        css="text-center"
    %}
</div>
{% endcapture %}
{% include new-includes/components/section.html
    content=banner-section
    css="py-6"
%}

{% capture fast-safe-expressive-section %}
<div class="text-center mb-20">
    <h2 class="text-3xl md:text-5xl font-bold text-gray-900 dark:text-white mb-6">
        Designed for Excellence
    </h2>
    <p class="text-xl text-gray-600 dark:text-gray-300 max-w-3xl mx-auto">
        Swift combines the best in modern language thinking with wisdom from the wider Apple engineering culture.
    </p>
</div>
<div class="grid-3-cols grid grid-cols-1 md:grid-cols-3 gap-12 text-center">
    <div class="p-6 rounded-xl bg-white dark:bg-gray-800 shadow-sm border border-orange-100 dark:border-orange-900/30 hover:shadow-md transition-shadow">
        <div class="inline-flex items-center justify-center h-16 w-16 rounded-full bg-orange-100 dark:bg-orange-900/30 text-orange-600 dark:text-orange-300 mb-4">
            <img src="/assets/images/new-images/icon-fast.png" class="h-10 w-10" />
        </div>
        <h3 class="text-xl font-semibold text-gray-900 dark:text-white mb-3">
            Fast
        </h3>
        <p class="text-gray-600 dark:text-gray-300">
            Swift aims to replace C-based languages and match their performance, while maintaining consistency and predictability.
        </p>
    </div>
    <div class="p-6 rounded-xl bg-white dark:bg-gray-800 shadow-sm border border-orange-100 dark:border-orange-900/30 hover:shadow-md transition-shadow">
        <div class="inline-flex items-center justify-center h-16 w-16 rounded-full bg-orange-100 dark:bg-orange-900/30 text-orange-600 dark:text-orange-300 mb-4">
            <img src="/assets/images/new-images/icon-safe.png" class="h-10 w-10" />
        </div>
        <h3 class="text-xl font-semibold text-gray-900 dark:text-white mb-3">
            Safe
        </h3>
        <p class="text-gray-600 dark:text-gray-300">
            Swift prioritizes safety and clarity, ensuring that code behaves in a safe manner while also promoting good practices.
        </p>
    </div>
    <div class="p-6 rounded-xl bg-white dark:bg-gray-800 shadow-sm border border-orange-100 dark:border-orange-900/30 hover:shadow-md transition-shadow">
        <div class="inline-flex items-center justify-center h-16 w-16 rounded-full bg-orange-100 dark:bg-orange-900/30 text-orange-600 dark:text-orange-300 mb-4">
            <img src="/assets/images/new-images/icon-expressive.png" class="h-10 w-10" />
        </div>
        <h3 class="text-xl font-semibold text-gray-900 dark:text-white mb-3">
            Expressive
        </h3>
        <p class="text-gray-600 dark:text-gray-300">
            Swift builds upon decades of advancements in computer science, providing a modern syntax that is a joy to use.
        </p>
    </div>
</div>
{% endcapture %}
{% include new-includes/components/section.html
    content=fast-safe-expressive-section
    style="orange"
    css="py-28 md:py-36 bg-orange-50 dark:bg-orange-900/20"
%}

{% capture use-cases-section %}
<div class="text-center mb-20">
    <h2 class="text-3xl md:text-5xl font-bold text-gray-900 dark:text-white mb-6">
        Use Cases
    </h2>
    <p class="text-xl text-gray-600 dark:text-gray-300 max-w-3xl mx-auto">
        Swift is used across multiple domains, from mobile apps to high-performance servers.
    </p>
</div>
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
    <a href="/getting-started/server/" class="group">
        <div class="h-full p-8 bg-white dark:bg-gray-800 rounded-xl shadow-sm border border-gray-200 dark:border-gray-700 flex flex-col hover:shadow-md hover:border-blue-200 dark:hover:border-blue-800 transition-all">
            <div class="flex items-center mb-4">
                <div class="flex items-center justify-center h-12 w-12 rounded-lg bg-blue-100 dark:bg-blue-900/30">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-blue-600 dark:text-blue-400" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M5 12h14M5 12a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v4a2 2 0 01-2 2M5 12a2 2 0 00-2 2v4a2 2 0 002 2h14a2 2 0 002-2v-4a2 2 0 00-2-2" />
                    </svg>
                </div>
                <h3 class="ml-4 text-xl font-semibold text-gray-900 dark:text-white group-hover:text-blue-600 dark:group-hover:text-blue-400 transition-colors">
                    Server & Networking
                </h3>
            </div>
            <p class="text-gray-600 dark:text-gray-300 flex-grow">
                Swift provides small memory footprint, quick startup time, and deterministic performance for server-side applications.
            </p>
            <div class="flex items-center mt-6 text-blue-600 dark:text-blue-400">
                <span class="text-sm font-medium">Learn more</span>
                <svg class="ml-2 w-4 h-4 transition-transform group-hover:translate-x-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path>
                </svg>
            </div>
        </div>
    </a>
    <a href="/getting-started/swiftui/" class="group">
        <div class="h-full p-8 bg-white dark:bg-gray-800 rounded-xl shadow-sm border border-gray-200 dark:border-gray-700 flex flex-col hover:shadow-md hover:border-pink-200 dark:hover:border-pink-800 transition-all">
            <div class="flex items-center mb-4">
                <div class="flex items-center justify-center h-12 w-12 rounded-lg bg-pink-100 dark:bg-pink-900/30">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-pink-600 dark:text-pink-400" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                        <rect x="6" y="2" width="12" height="20" rx="3" />
                        <path d="M10 4h4" />
                    </svg>
                </div>
                <h3 class="ml-4 text-xl font-semibold text-gray-900 dark:text-white group-hover:text-pink-600 dark:group-hover:text-pink-400 transition-colors">
                    Apple Platforms
                </h3>
            </div>
            <p class="text-gray-600 dark:text-gray-300 flex-grow">
                Swift is optimized when running on iOS, macOS, watchOS, and tvOS with full access to platform features.
            </p>
            <div class="flex items-center mt-6 text-pink-600 dark:text-pink-400">
                <span class="text-sm font-medium">Learn more</span>
                <svg class="ml-2 w-4 h-4 transition-transform group-hover:translate-x-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path>
                </svg>
            </div>
        </div>
    </a>

    <a href="/getting-started/cli-swiftpm/" class="group">
        <div class="h-full p-8 bg-white dark:bg-gray-800 rounded-xl shadow-sm border border-gray-200 dark:border-gray-700 flex flex-col hover:shadow-md hover:border-purple-200 dark:hover:border-purple-800 transition-all">
            <div class="flex items-center mb-4">
                <div class="flex items-center justify-center h-12 w-12 rounded-lg bg-purple-100 dark:bg-purple-900/30">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-purple-600 dark:text-purple-400" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M8 9l3 3-3 3m5 0h6" />
                    </svg>
                </div>
                <h3 class="ml-4 text-xl font-semibold text-gray-900 dark:text-white group-hover:text-purple-600 dark:group-hover:text-purple-400 transition-colors">
                    Cross-platform CLI
                </h3>
            </div>
            <p class="text-gray-600 dark:text-gray-300 flex-grow">
                Create command-line tools that run lightning-fast on Linux, macOS, and Windows platforms.
            </p>
            <div class="flex items-center mt-6 text-purple-600 dark:text-purple-400">
                <span class="text-sm font-medium">Learn more</span>
                <svg class="ml-2 w-4 h-4 transition-transform group-hover:translate-x-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path>
                </svg>
            </div>
        </div>
    </a>
</div>
{% endcapture %}
{% include new-includes/components/section.html
    content=use-cases-section
    css="py-28 md:py-36"
%}

{% capture packages-section %}
<div class="text-center mb-20">
    <h2 class="text-3xl md:text-5xl font-bold text-gray-900 dark:text-white mb-6">
        Package Ecosystem
    </h2>
    <p class="text-xl text-gray-600 dark:text-gray-300 max-w-3xl mx-auto">
        The Swift package ecosystem has thousands of packages to help you with all kinds of tasks across your projects.
    </p>
</div>

<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 mb-16">
    <!-- Featured Package 1 -->
    <div class="p-6 bg-white dark:bg-gray-800 rounded-xl shadow-sm border border-gray-200 dark:border-gray-700 hover:shadow-md transition-shadow">
        <div class="flex items-center justify-between mb-4">
            <h3 class="text-lg font-semibold text-gray-900 dark:text-white">ArgumentParser</h3>
            <span class="inline-flex items-center px-2.5 py-0.5 rounded-full text-xs font-medium bg-blue-100 text-blue-800 dark:bg-blue-900/30 dark:text-blue-300">Official</span>
        </div>
        <p class="text-gray-600 dark:text-gray-300 text-sm mb-4">
            Straightforward, type-safe argument parsing for Swift.
        </p>
        <div class="flex justify-between items-center">
            <a href="https://github.com/apple/swift-argument-parser" target="_blank" class="text-blue-600 dark:text-blue-400 text-sm flex items-center hover:underline">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4" />
                </svg>
                View Repository
            </a>
            <div class="flex items-center text-gray-500 dark:text-gray-400 text-xs">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
                </svg>
                Command-line
            </div>
        </div>
    </div>

    <!-- Featured Package 2 -->
    <div class="p-6 bg-white dark:bg-gray-800 rounded-xl shadow-sm border border-gray-200 dark:border-gray-700 hover:shadow-md transition-shadow">
        <div class="flex items-center justify-between mb-4">
            <h3 class="text-lg font-semibold text-gray-900 dark:text-white">SwiftNIO</h3>
            <span class="inline-flex items-center px-2.5 py-0.5 rounded-full text-xs font-medium bg-blue-100 text-blue-800 dark:bg-blue-900/30 dark:text-blue-300">Official</span>
        </div>
        <p class="text-gray-600 dark:text-gray-300 text-sm mb-4">
            Event-driven network application framework for high performance.
        </p>
        <div class="flex justify-between items-center">
            <a href="https://github.com/apple/swift-nio" target="_blank" class="text-blue-600 dark:text-blue-400 text-sm flex items-center hover:underline">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4" />
                </svg>
                View Repository
            </a>
            <div class="flex items-center text-gray-500 dark:text-gray-400 text-xs">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
                </svg>
                Networking
            </div>
        </div>
    </div>

    <!-- Featured Package 3 -->
    <div class="p-6 bg-white dark:bg-gray-800 rounded-xl shadow-sm border border-gray-200 dark:border-gray-700 hover:shadow-md transition-shadow">
        <div class="flex items-center justify-between mb-4">
            <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Algorithms</h3>
            <span class="inline-flex items-center px-2.5 py-0.5 rounded-full text-xs font-medium bg-blue-100 text-blue-800 dark:bg-blue-900/30 dark:text-blue-300">Official</span>
        </div>
        <p class="text-gray-600 dark:text-gray-300 text-sm mb-4">
            Swift implementations of common algorithms and data structures.
        </p>
        <div class="flex justify-between items-center">
            <a href="https://github.com/apple/swift-algorithms" target="_blank" class="text-blue-600 dark:text-blue-400 text-sm flex items-center hover:underline">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4" />
                </svg>
                View Repository
            </a>
            <div class="flex items-center text-gray-500 dark:text-gray-400 text-xs">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
                </svg>
                Data Structures
            </div>
        </div>
    </div>

    <!-- Featured Package 4 -->
    <div class="p-6 bg-white dark:bg-gray-800 rounded-xl shadow-sm border border-gray-200 dark:border-gray-700 hover:shadow-md transition-shadow">
        <div class="flex items-center justify-between mb-4">
            <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Vapor</h3>
            <span class="inline-flex items-center px-2.5 py-0.5 rounded-full text-xs font-medium bg-green-100 text-green-800 dark:bg-green-900/30 dark:text-green-300">Community</span>
        </div>
        <p class="text-gray-600 dark:text-gray-300 text-sm mb-4">
            A server-side Swift web framework.
        </p>
        <div class="flex justify-between items-center">
            <a href="https://github.com/vapor/vapor" target="_blank" class="text-blue-600 dark:text-blue-400 text-sm flex items-center hover:underline">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4" />
                </svg>
                View Repository
            </a>
            <div class="flex items-center text-gray-500 dark:text-gray-400 text-xs">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
                </svg>
                Web Framework
            </div>
        </div>
    </div>
</div>

<div class="text-center">
    <a href="/packages/" class="inline-flex items-center px-6 py-3 border border-transparent text-base font-medium rounded-md shadow-sm text-white bg-gray-900 hover:bg-gray-800 dark:bg-gray-700 dark:hover:bg-gray-600 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-500 transition-colors">
        Explore More Packages
        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 ml-2" viewBox="0 0 20 20" fill="currentColor">
            <path fill-rule="evenodd" d="M10.293 5.293a1 1 0 011.414 0l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414-1.414L12.586 11H5a1 1 0 110-2h7.586l-2.293-2.293a1 1 0 010-1.414z" clip-rule="evenodd" />
        </svg>
    </a>
</div>
{% endcapture %}
{% include new-includes/components/section.html
    content=packages-section
    style="yellow"
    css="py-28 md:py-36 bg-yellow-50 dark:bg-yellow-900/20"
%}

{% capture community-section %}
<div class="text-center mb-20">
    <h2 class="text-3xl md:text-5xl font-bold text-gray-900 dark:text-white mb-6">
        Join the Community
    </h2>
    <p class="text-xl text-gray-600 dark:text-gray-300 max-w-3xl mx-auto">
        Swift has a vibrant community of developers who contribute to the language and help each other.
    </p>
</div>

<div class="grid grid-cols-1 md:grid-cols-2 gap-12">
    <div class="bg-white dark:bg-gray-800 rounded-xl shadow-sm border border-gray-200 dark:border-gray-700 overflow-hidden">
        <div class="p-8">
            <div class="flex items-center mb-4">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10 text-purple-600 dark:text-purple-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8h2a2 2 0 012 2v6a2 2 0 01-2 2h-2v4l-4-4H9a1.994 1.994 0 01-1.414-.586m0 0L11 14h4a2 2 0 002-2V6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2v4l.586-.586z" />
                </svg>
                <h3 class="ml-4 text-2xl font-semibold text-gray-900 dark:text-white">
                    Forums
                </h3>
            </div>
            <p class="text-gray-600 dark:text-gray-300 mb-6">
                The official Swift forums are the best place to discuss Swift evolution proposals, language features, and development.
            </p>
            <ul class="space-y-3 mb-6">
                <li class="flex items-center text-gray-600 dark:text-gray-300">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2 text-green-500 dark:text-green-400" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                    </svg>
                    Engage with language development
                </li>
                <li class="flex items-center text-gray-600 dark:text-gray-300">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2 text-green-500 dark:text-green-400" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                    </svg>
                    Get help from experienced developers
                </li>
                <li class="flex items-center text-gray-600 dark:text-gray-300">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2 text-green-500 dark:text-green-400" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                    </svg>
                    Share your Swift projects
                </li>
            </ul>
            <a href="https://forums.swift.org" target="_blank" class="inline-flex items-center px-5 py-2 border border-transparent text-base font-medium rounded-md shadow-sm text-white bg-purple-600 hover:bg-purple-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-purple-500 transition-colors">
                Visit the Forums
            </a>
        </div>
    </div>
    
    <div class="bg-white dark:bg-gray-800 rounded-xl shadow-sm border border-gray-200 dark:border-gray-700 overflow-hidden">
        <div class="p-8">
            <div class="flex items-center mb-4">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10 text-blue-600 dark:text-blue-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4M7.835 4.697a3.42 3.42 0 001.946-.806 3.42 3.42 0 014.438 0 3.42 3.42 0 001.946.806 3.42 3.42 0 013.138 3.138 3.42 3.42 0 00.806 1.946 3.42 3.42 0 010 4.438 3.42 3.42 0 00-.806 1.946 3.42 3.42 0 01-3.138 3.138 3.42 3.42 0 00-1.946.806 3.42 3.42 0 01-4.438 0 3.42 3.42 0 00-1.946-.806 3.42 3.42 0 01-3.138-3.138 3.42 3.42 0 00-.806-1.946 3.42 3.42 0 010-4.438 3.42 3.42 0 00.806-1.946 3.42 3.42 0 013.138-3.138z" />
                </svg>
                <h3 class="ml-4 text-2xl font-semibold text-gray-900 dark:text-white">
                    Contribute
                </h3>
            </div>
            <p class="text-gray-600 dark:text-gray-300 mb-6">
                Swift is an open-source project and welcomes contributions from everyone. There are many ways to contribute beyond writing code.
            </p>
            <ul class="space-y-3 mb-6">
                <li class="flex items-center text-gray-600 dark:text-gray-300">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2 text-green-500 dark:text-green-400" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                    </svg>
                    Submit bug fixes and features
                </li>
                <li class="flex items-center text-gray-600 dark:text-gray-300">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2 text-green-500 dark:text-green-400" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                    </svg>
                    Improve documentation
                </li>
                <li class="flex items-center text-gray-600 dark:text-gray-300">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2 text-green-500 dark:text-green-400" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                    </svg>
                    Join workgroups
                </li>
            </ul>
            <a href="/contributing/" class="inline-flex items-center px-5 py-2 border border-transparent text-base font-medium rounded-md shadow-sm text-white bg-blue-600 hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-500 transition-colors">
                Learn How to Contribute
            </a>
        </div>
    </div>
</div>
{% endcapture %}
{% include new-includes/components/section.html
    content=community-section
    css="py-28 md:py-36"
%}

{% capture case-studies-section %}
<div class="text-center mb-20">
    <h2 class="text-3xl md:text-5xl font-bold text-gray-900 dark:text-white mb-6">
        Success Stories
    </h2>
    <p class="text-xl text-gray-600 dark:text-gray-300 max-w-3xl mx-auto">
        Companies and developers around the world use Swift to build powerful applications and solve real-world problems.
    </p>
</div>

<div class="grid grid-cols-1 md:grid-cols-2 gap-8">
    <div class="relative rounded-xl overflow-hidden bg-white dark:bg-gray-800 shadow-lg">
        <div class="h-1 bg-gradient-to-r from-blue-600 to-indigo-600"></div>
        <div class="relative p-8 md:p-10 flex flex-col h-full">
            <div class="flex items-center mb-6">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-12 w-12 text-blue-600 dark:text-blue-400" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1.5">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z" />
                </svg>
                <h3 class="ml-4 text-2xl font-bold text-gray-900 dark:text-white">
                    Things Cloud
                </h3>
            </div>
            <p class="text-gray-600 dark:text-gray-300 text-lg mb-6">
                "Swift on the server has been transformational for our backend. Our latest cloud infrastructure is entirely built with Swift, delivering better performance with less code."
            </p>
            <div class="mt-auto">
                <span class="inline-flex items-center px-3 py-1 rounded-full text-sm font-medium bg-blue-100 dark:bg-blue-900/30 text-blue-800 dark:text-blue-300">
                    Server-side Swift
                </span>
            </div>
            <div class="mt-4">
                <a href="/blog/how-swifts-server-support-powers-things-cloud/" class="inline-flex items-center text-sm font-medium text-blue-600 dark:text-blue-400 hover:text-blue-700 dark:hover:text-blue-300">
                    Read the case study
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 ml-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3" />
                    </svg>
                </a>
            </div>
        </div>
    </div>

    <div class="relative rounded-xl overflow-hidden bg-white dark:bg-gray-800 shadow-lg">
        <div class="h-1 bg-gradient-to-r from-purple-600 to-pink-500"></div>
        <div class="relative p-8 md:p-10 flex flex-col h-full">
            <div class="flex items-center mb-6">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-12 w-12 text-purple-600 dark:text-purple-400" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1.5">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M19.428 15.428a2 2 0 00-1.022-.547l-2.387-.477a6 6 0 00-3.86.517l-.318.158a6 6 0 01-3.86.517L6.05 15.21a2 2 0 00-1.806.547M8 4h8l-1 1v5.172a2 2 0 00.586 1.414l5 5c1.26 1.26.367 3.414-1.415 3.414H4.828c-1.782 0-2.674-2.154-1.414-3.414l5-5A2 2 0 009 10.172V5L8 4z" />
                </svg>
                <h3 class="ml-4 text-2xl font-bold text-gray-900 dark:text-white">
                    MLX Swift
                </h3>
            </div>
            <p class="text-gray-600 dark:text-gray-300 text-lg mb-6">
                "With MLX Swift, we've created a productive environment for machine learning research that combines the performance of MLX with Swift's expressivity and safety."
            </p>
            <div class="mt-auto">
                <span class="inline-flex items-center px-3 py-1 rounded-full text-sm font-medium bg-purple-100 dark:bg-purple-900/30 text-purple-800 dark:text-purple-300">
                    Machine Learning
                </span>
            </div>
            <div class="mt-4">
                <a href="/blog/mlx-swift/" class="inline-flex items-center text-sm font-medium text-purple-600 dark:text-purple-400 hover:text-purple-700 dark:hover:text-purple-300">
                    Read the case study
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 ml-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3" />
                    </svg>
                </a>
            </div>
        </div>
    </div>
</div>
{% endcapture %}
{% include new-includes/components/section.html
    content=case-studies-section
    css="py-28 md:py-36 bg-gray-50 dark:bg-gray-800/50"
%}

{% capture links-section %}
<div class="text-center mb-20">
    <h2 class="text-3xl md:text-5xl font-bold text-gray-900 dark:text-white mb-6">
        Resources
    </h2>
    <p class="text-xl text-gray-600 dark:text-gray-300 max-w-3xl mx-auto">
        Explore more Swift resources to help with your development journey.
    </p>
</div>

<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-x-8 gap-y-10">
    <div>
        <h3 class="text-lg font-semibold text-gray-900 dark:text-white mb-4">Learn Swift</h3>
        <ul class="space-y-3">
            <li>
                <a href="https://docs.swift.org/swift-book/" class="text-blue-600 dark:text-blue-400 hover:underline">The Swift Programming Language</a>
            </li>
            <li>
                <a href="/documentation/api-design-guidelines/" class="text-blue-600 dark:text-blue-400 hover:underline">API Design Guidelines</a>
            </li>
            <li>
                <a href="/getting-started/" class="text-blue-600 dark:text-blue-400 hover:underline">Getting Started Guide</a>
            </li>
            <li>
                <a href="/documentation/articles/" class="text-blue-600 dark:text-blue-400 hover:underline">Swift Articles</a>
            </li>
        </ul>
    </div>

    <div>
        <h3 class="text-lg font-semibold text-gray-900 dark:text-white mb-4">Development</h3>
        <ul class="space-y-3">
            <li>
                <a href="/documentation/package-manager/" class="text-blue-600 dark:text-blue-400 hover:underline">Swift Package Manager</a>
            </li>
            <li>
                <a href="/documentation/server/" class="text-blue-600 dark:text-blue-400 hover:underline">Server-side Swift</a>
            </li>
            <li>
                <a href="/packages/" class="text-blue-600 dark:text-blue-400 hover:underline">Swift Packages</a>
            </li>
            <li>
                <a href="/tools/" class="text-blue-600 dark:text-blue-400 hover:underline">Development Tools</a>
            </li>
        </ul>
    </div>

    <div>
        <h3 class="text-lg font-semibold text-gray-900 dark:text-white mb-4">Community</h3>
        <ul class="space-y-3">
            <li>
                <a href="https://forums.swift.org" class="text-blue-600 dark:text-blue-400 hover:underline">Swift Forums</a>
            </li>
            <li>
                <a href="/blog/" class="text-blue-600 dark:text-blue-400 hover:underline">Swift Blog</a>
            </li>
            <li>
                <a href="/contributing/" class="text-blue-600 dark:text-blue-400 hover:underline">Contributing to Swift</a>
            </li>
            <li>
                <a href="/community/" class="text-blue-600 dark:text-blue-400 hover:underline">Community Guidelines</a>
            </li>
        </ul>
    </div>
</div>
{% endcapture %}
{% include new-includes/components/section.html
    content=links-section
    css="py-28 md:py-36 bg-gray-100 dark:bg-gray-800"
%}
