<script lang="ts">
    import { Input } from '$lib/components/ui/input';
    import { Textarea } from '$lib/components/ui/textarea';
    import { Button } from '$lib/components/ui/button';
    import CheckCheck from 'lucide-svelte/icons/check-check';
    import { Home, PlayIcon, PhoneOutgoingIcon, MessageCircle } from 'lucide-svelte/icons';
    import { fly } from 'svelte/transition';
</script>

<div class="flex flex-col min-h-screen">
    <header class="px-4 lg:px-6 h-14 flex items-center bg-sky-400">
        <a href="#" class="flex items-center justify-center">
            <img src="/logo.png" alt="" width="64" class="mt-8" />
        </a>
        <nav class="ml-auto flex gap-2 sm:gap-4 font-medium">
            <a href="#" class="text-sm bg-white p-1 rounded-md hover:underline underline-offset-4"> About </a>
            <a href="#" class="text-sm bg-white p-1 rounded-md hover:underline underline-offset-4"> Services </a>
            <a href="#" class="text-sm bg-white p-1 rounded-md hover:underline underline-offset-4"> Partners </a>
            <a href="#" class="text-sm bg-white p-1 rounded-md hover:underline underline-offset-4"> Location</a>
        </nav>
    </header>
    <main class="flex-1 flex-wrap">
        <section class="py-12 md:py-24 lg:py-32 xl:py-48">
            <div class="px-4 md:px-6">
                <div class="space-y-2">
                    <h1 class="text-3xl font-bold tracking-tighter sm:text-5xl xl:text-6xl">Pranav Waterproofing Solutions for Your <Home class="inline" /></h1>
                    <p class="text-gray-500 md:text-xl dark:text-gray-400">
                        Water Leakage? Protect your home from water damage with our high-quality waterproofing products and services.
                    </p>
                </div>
                <div class="mt-4 flex justify-between space-x-2">
                    <a
                        href="https://wa.me/+919642518564?text=Hi%20i%20live%20at%20ADDRESS%20i%20want%20to%20book%20a%20inspection%20visit%20for%20PROBLEM%20can%20i%20call?"
                        class="flex-1 flex items-center justify-center rounded-md bg-green-500 p-3 font-semibold shadow-neutral-400 shadow-md text-gray-50 transition-colors hover:bg-gray-900/90 focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-gray-950 disabled:pointer-events-none disabled:opacity-50 dark:bg-gray-50 dark:text-gray-900 dark:hover:bg-gray-50/90 dark:focus-visible:ring-gray-300"
                    >
                        <MessageCircle class="w-4 h-4 me-2" /> WhatsApp
                    </a>
                    <a
                        href="tel:9642518564"
                        class="flex-1 flex items-center justify-center  rounded-md bg-sky-400 p-3 font-semibold shadow-neutral-400 shadow-md text-gray-50 transition-colors hover:bg-gray-900/90 focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-gray-950 disabled:pointer-events-none disabled:opacity-50 dark:bg-gray-50 dark:text-gray-900 dark:hover:bg-gray-50/90 dark:focus-visible:ring-gray-300"
                    >
                        <PhoneOutgoingIcon class="w-4 h-4 me-2" /> 9642518564
                    </a>
                    <a
                        href="https://www.facebook.com/profile.php?id=100083087423019&paipv=0&eav=AfbIdgEzrQFs9ZZ_5lUka2yO5p3_VmFjJttfPGJ2P-DIvftIw6nU4KL6H1pJi_WEAMM"
                        class="flex items-center justify-center rounded-md bg-blue-500 p-3 font-semibold shadow-neutral-400 shadow-md text-gray-50 transition-colors hover:bg-gray-900/90 focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-gray-950 disabled:pointer-events-none disabled:opacity-50 dark:bg-gray-50 dark:text-gray-900 dark:hover:bg-gray-50/90 dark:focus-visible:ring-gray-300"
                    >
                        <img src="https://upload.wikimedia.org/wikipedia/commons/5/51/Facebook_f_logo_%282019%29.svg" alt="Facebook" class="w-4 h-4" />
                    </a>
                </div>

                <img src="pranav-banner.jpg" alt="" class="w-full object-cover object-center rounded-lg shadow-md mt-4" />
            </div>
        </section>
        <section class="py-12 md:py-24 lg:py-32 bg-gradient-to-r from-sky-300 via-sky-400 to-sky-500">
            <div class="container px-4 md:px-6">
                <div class="flex flex-col justify-center space-y-3">
                    <div class="space-y-2">
                        <h2 class="text-3xl font-bold tracking-tighter sm:text-4xl">Terrace Waterproofing</h2>
                        <p class="text-white md:text-xl/relaxed lg:text-base/relaxed xl:text-xl/relaxed dark:text-gray-400">
                            Protect your roof from water damage and extend its lifespan with our professional waterproofing services.
                        </p>
                    </div>
                    <ul class="grid gap-2 pt-3">
                        <li class="flex items-center space-x-2 bg-white rounded-md p-2">
                            <CheckCheck class="h-5 w-5 text-green-500" />
                            <span>Prevent leaks and water intrusion</span>
                        </li>
                        <li class="flex items-center space-x-2 bg-white rounded-md p-2">
                            <CheckCheck class="h-5 w-5 text-green-500" />
                            <span>Improve energy efficiency</span>
                        </li>
                        <li class="flex items-center space-x-2 bg-white rounded-md p-2">
                            <CheckCheck class="h-5 w-5 text-green-500" />
                            <span>Extend the life of your roof</span>
                        </li>
                    </ul>
                    <a
                        href="#"
                        class="inline-flex h-10 items-center justify-center rounded-md bg-gray-900 px-8 text-sm font-medium text-gray-50 shadow transition-colors hover:bg-gray-900/90 focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-gray-950 disabled:pointer-events-none disabled:opacity-50 dark:bg-gray-50 dark:text-gray-900 dark:hover:bg-gray-50/90 dark:focus-visible:ring-gray-300"
                    >
                        Watch Video <PlayIcon class="ml-1 h-4 w-4" />
                    </a>
                    <img
                        src="gallery-roof.webp"
                        width="550"
                        height="310"
                        alt="Roof Waterproofing"
                        class="mx-auto aspect-video overflow-hidden rounded-xl object-cover object-center sm:w-full lg:order-last fade-in shadow-md"
                    />
                </div>
            </div>
        </section>

        <section class="py-12 md:py-24 lg:py-32 bg-black-gradient">
            <div class="container px-4 md:px-6">
                <div class="flex flex-col justify-center space-y-3">
                    <div class="space-y-2">
                        <h2 class="text-3xl font-bold tracking-tighter sm:text-4xl text-white">Exterior Waterproofing</h2>
                        <p class="text-gray-500 md:text-xl/relaxed lg:text-base/relaxed xl:text-xl/relaxed dark:text-gray-400">
                            Protect your exteriors from monsoon damage with our high-performance waterproofing solutions.
                        </p>
                    </div>
                    <ul class="grid gap-2 pt-3">
                        <li class="flex items-center space-x-2 bg-white rounded-md p-2">
                            <CheckCheck class="h-5 w-5 text-green-500" />
                            <span>Prevent leaks and moisture buildup</span>
                        </li>
                        <li class="flex items-center space-x-2 bg-white rounded-md p-2">
                            <CheckCheck class="h-5 w-5 text-green-500" />
                            <span>Improve indoor air quality</span>
                        </li>
                        <li class="flex items-center space-x-2 bg-white rounded-md p-2">
                            <CheckCheck class="h-5 w-5 text-green-500" />
                            <span>Increase the value of your home</span>
                        </li>
                    </ul>
                    <a
                        href="#"
                        class="inline-flex h-10 items-center justify-center rounded-md bg-sky-400 px-8 text-sm font-medium text-gray-50 shadow transition-colors hover:bg-gray-900/90 focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-gray-950 disabled:pointer-events-none disabled:opacity-50 dark:bg-gray-50 dark:text-gray-900 dark:hover:bg-gray-50/90 dark:focus-visible:ring-gray-300"
                    >
                        Watch Video <PlayIcon class="ml-1 h-4 w-4" />
                    </a>
                    <img
                        src="gallery-basement.webp"
                        width="550"
                        height="310"
                        alt="Basement Waterproofing"
                        class="mx-auto aspect-video overflow-hidden rounded-xl object-cover object-center sm:w-full lg:order-last fade-in shadow-md"
                    />
                </div>
            </div>
        </section>

        <style>
            .bg-black-gradient {
                background: linear-gradient(240deg, rgba(0, 0, 0, 0.8), rgba(0, 0, 0, 1));
            }
        </style>

        <section class="py-12 md:py-24 lg:py-32 bg-gray-200">
            <div class="container px-4 md:px-6">
                <div class="flex flex-col justify-center space-y-3">
                    <div class="space-y-2">
                        <h2 class="text-3xl font-bold tracking-tighter sm:text-4xl">Watertank Waterproofing</h2>
                        <p class="text-gray-500 md:text-xl/relaxed lg:text-base/relaxed xl:text-xl/relaxed dark:text-gray-400">
                            Ensure your watertank remains leak-proof and durable with our advanced waterproofing solutions.
                        </p>
                    </div>
                    <ul class="grid gap-2 pt-3">
                        <li class="flex items-center space-x-2 bg-white rounded-md p-2">
                            <CheckCheck class="h-5 w-5 text-green-500" />
                            <span>Ultimate Leak Protection</span>
                        </li>
                        <li class="flex items-center space-x-2 bg-white rounded-md p-2">
                            <CheckCheck class="h-5 w-5 text-green-500" />
                            <span>Long-Lasting Durability</span>
                        </li>
                        <li class="flex items-center space-x-2 bg-white rounded-md p-2">
                            <CheckCheck class="h-5 w-5 text-green-500" />
                            <span>Eco-Friendly Options</span>
                        </li>
                        <li class="flex items-center space-x-2 bg-white rounded-md p-2">
                            <CheckCheck class="h-5 w-5 text-green-500" />
                            <span>No Hazardous chemicals</span>
                        </li>
                    </ul>
                    <a
                        href="#"
                        class="inline-flex h-10 items-center justify-center rounded-md bg-gray-900 px-8 text-sm font-medium text-gray-50 shadow transition-colors hover:bg-gray-900/90 focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-gray-950 disabled:pointer-events-none disabled:opacity-50 dark:bg-gray-50 dark:text-gray-900 dark:hover:bg-gray-50/90 dark:focus-visible:ring-gray-300"
                    >
                        Watch Video <PlayIcon class="ml-1 h-4 w-4" />
                    </a>
                    <img
                        src="gallery-watertank.webp"
                        width="550"
                        height="310"
                        alt="Watertank Waterproofing"
                        class="mx-auto aspect-video overflow-hidden rounded-xl object-cover object-center sm:w-full lg:order-last fade-in shadow-md"
                    />
                </div>
            </div>
        </section>
        <section class="py-12 md:py-24 lg:py-32 bg-white raindrop-gradient bg-no-repeat bg-cover bg-center" style="background-image: url(watersplash.webp);">
            <div class="container px-4 md:px-6">
                <div class="flex flex-col justify-center space-y-3">
                    <div class="space-y-2">
                        <h2 class="text-3xl font-bold tracking-tighter sm:text-4xl text-white">Wet Areas Waterproofing</h2>
                        <p class="text-gray-200 md:text-xl/relaxed lg:text-base/relaxed xl:text-xl/relaxed dark:text-gray-400">
                            Keep your kitchen and bathrooms dry and safe with our easy waterproofing solutions.
                        </p>
                    </div>
                    <ul class="grid gap-2 pt-3">
                        <li class="flex items-center space-x-2 bg-white rounded-md p-2">
                            <CheckCheck class="h-5 w-5 text-green-500" />
                            <span>Stops leaks</span>
                        </li>
                        <li class="flex items-center space-x-2 bg-white rounded-md p-2">
                            <CheckCheck class="h-5 w-5 text-green-500" />
                            <span>Prevents mold</span>
                        </li>
                        <li class="flex items-center space-x-2 bg-white rounded-md p-2">
                            <CheckCheck class="h-5 w-5 text-green-500" />
                            <span>Easy to apply</span>
                        </li>
                        <li class="flex items-center space-x-2 bg-white rounded-md p-2">
                            <CheckCheck class="h-5 w-5 text-green-500" />
                            <span>Safe for families</span>
                        </li>
                    </ul>
                    <a
                        href="#"
                        class="inline-flex h-10 items-center justify-center rounded-md bg-gray-900 px-8 text-sm font-medium text-gray-50 shadow transition-colors hover:bg-gray-900/90 focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-gray-950 disabled:pointer-events-none disabled:opacity-50 dark:bg-gray-50 dark:text-gray-900 dark:hover:bg-gray-50/90 dark:focus-visible:ring-gray-300"
                    >
                        Watch Video <PlayIcon class="ml-1 h-4 w-4" />
                    </a>
                    <img
                        src="gallery-general.webp"
                        width="550"
                        height="310"
                        alt="Wet Areas Waterproofing"
                        class="mx-auto aspect-video overflow-hidden rounded-xl object-cover object-center sm:w-full lg:order-last fade-in shadow-md"
                    />
                </div>
            </div>
        </section>

        <section class="py-12 md:py-24 lg:py-32 bg-gray-100 dark:bg-gray-800">
            <div class="container px-4 md:px-6">
                <div class="flex flex-col items-center justify-center space-y-4 text-center">
                    <div class="space-y-2">
                        <h2 class="text-3xl font-bold tracking-tighter sm:text-4xl">Locate Us</h2>
                        <p class="text-gray-500 md:text-xl/relaxed lg:text-base/relaxed xl:text-xl/relaxed dark:text-gray-400">
                            Find our offices at the address below on the map. Drop by to learn more about our waterproofing solutions.
                        </p>
                    </div>
                    <div class="w-full md:w-3/4 lg:w-1/2">
                        <!-- Embedded Google Map -->
                        <iframe
                            src="https://maps.google.com/maps?width=100%25&amp;height=600&amp;hl=en&amp;q=Gayatri%20Homes,%20Plot%20no.%2099,%20Gayatri%20Nagar%20Rd,%20Srinivasa%20Gayatri%20Nagar,%20Kharmanghat,%20Hyderabad,%20Telangana%20500079+()&amp;t=&amp;z=14&amp;ie=UTF8&amp;iwloc=B&amp;output=embed"
                            width="100%"
                            height="450"
                            style="border:0;"
                            allowfullscreen=""
                            loading="lazy"
                            class=" rounded-2xl shadow-lg"
                        ></iframe>
                    </div>
                </div>
            </div>
        </section>
    </main>
    <footer class="flex flex-col gap-2 sm:flex-row py-6 w-full shrink-0 items-center px-4 md:px-6 border-t">
        <p class="text-xs text-gray-500 dark:text-gray-400">&copy; 2024 Pranav Waterproofing Solutions. All rights reserved.</p>
        <nav class="sm:ml-auto flex gap-4 sm:gap-6">
            <a href="#" class="text-xs hover:underline underline-offset-4"> Terms of Service </a>
            <a href="#" class="text-xs hover:underline underline-offset-4"> Privacy Policy </a>
        </nav>
    </footer>
</div>

<style>
    /* Optional: Add some padding around the pattern to make it cleaner */
</style>
