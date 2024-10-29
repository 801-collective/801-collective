<template>
  <div class="min-h-screen bg-gradient-to-b from-gray-50 to-white">
    <!-- Navigation -->
    <nav class="fixed w-full bg-white/80 backdrop-blur-sm shadow-sm z-50">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex justify-between items-center h-16">
          <div class="flex-shrink-0">
            <h1 class="text-2xl font-bold text-indigo-600">801 Collective</h1>
          </div>
          <div class="hidden md:block">
            <div class="ml-10 flex items-center space-x-4">
              <a href="#features" class="text-gray-700 hover:text-indigo-600 px-3 py-2">Features</a>
              <a href="#benefits" class="text-gray-700 hover:text-indigo-600 px-3 py-2">Benefits</a>
              <a href="#testimonials" class="text-gray-700 hover:text-indigo-600 px-3 py-2">Success Stories</a>
              <button class="bg-indigo-600 text-white px-4 py-2 rounded-lg hover:bg-indigo-700 transition">
                Sign Up
              </button>
            </div>
          </div>
        </div>
      </div>
    </nav>

    <!-- Hero Section -->
    <div class="pt-24 pb-16 sm:pt-32 relative overflow-hidden">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center">
          <h2 class="text-4xl font-bold tracking-tight text-gray-900 sm:text-6xl">
            Grow Your Local Business Online
          </h2>
          <p class="mt-6 text-lg leading-8 text-gray-600 max-w-2xl mx-auto">
            Join 801 Collective and connect with customers looking for authentic, local products.
            We help small businesses thrive in the digital marketplace.
          </p>
          <div class="mt-10 flex items-center justify-center gap-x-6">
            <button class="rounded-md bg-indigo-600 px-6 py-3 text-lg font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">
              Get Started
            </button>
            <button class="text-lg font-semibold leading-6 text-gray-900 hover:text-indigo-600">
              Learn more <span aria-hidden="true">→</span>
            </button>
          </div>
        </div>
      </div>
    </div>

    <!-- Features Section -->
    <div id="features" class="py-24 bg-white sm:py-32">
      <div class="max-w-7xl mx-auto px-6 lg:px-8">
        <div class="mx-auto max-w-2xl lg:text-center">
          <h2 class="text-base font-semibold leading-7 text-indigo-600">Features</h2>
          <p class="mt-2 text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
            Everything you need to succeed online
          </p>
        </div>
        <div class="mx-auto mt-16 max-w-2xl sm:mt-20 lg:mt-24 lg:max-w-none">
          <dl class="grid max-w-xl grid-cols-1 gap-x-8 gap-y-16 lg:max-w-none lg:grid-cols-3">
            <div class="flex flex-col">
              <dt class="font-semibold leading-7 text-gray-900 text-lg">
                Easy Setup & Management
              </dt>
              <dd class="mt-4 flex flex-auto flex-col text-base leading-7 text-gray-600">
                <p>Set up your online store in minutes. Manage inventory, orders, and customer relationships all in one place.</p>
              </dd>
            </div>
            <div class="flex flex-col">
              <dt class="font-semibold leading-7 text-gray-900 text-lg">
                Local Market Focus
              </dt>
              <dd class="mt-4 flex flex-auto flex-col text-base leading-7 text-gray-600">
                <p>Connect with customers in your area who value local businesses and authentic products.</p>
              </dd>
            </div>
            <div class="flex flex-col">
              <dt class="font-semibold leading-7 text-gray-900 text-lg">
                Marketing Tools
              </dt>
              <dd class="mt-4 flex flex-auto flex-col text-base leading-7 text-gray-600">
                <p>Built-in marketing tools to help you reach more customers and grow your business.</p>
              </dd>
            </div>
          </dl>
        </div>
      </div>
    </div>

    <!-- Benefits Section -->
    <div id="benefits" class="py-24 bg-gray-50 sm:py-32">
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div class="mx-auto max-w-2xl lg:text-center">
          <h2 class="text-base font-semibold leading-7 text-indigo-600">Benefits</h2>
          <p class="mt-2 text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
            Why Choose 801 Collective?
          </p>
        </div>
        <div class="mx-auto mt-16 max-w-2xl sm:mt-20 lg:mt-24 lg:max-w-none">
          <div class="grid grid-cols-1 gap-8 lg:grid-cols-2">
            <div class="relative pl-16">
              <div class="absolute left-0 top-0 flex h-10 w-10 items-center justify-center rounded-lg bg-indigo-600">
                <svg class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M12 6v12m-3-2.818l.879.659c1.171.879 3.07.879 4.242 0 1.172-.879 1.172-2.303 0-3.182C13.536 12.219 12.768 12 12 12c-.725 0-1.45-.22-2.003-.659-1.106-.879-1.106-2.303 0-3.182s2.9-.879 4.006 0l.415.33M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                </svg>
              </div>
              <dt class="text-lg font-semibold leading-7 text-gray-900">
                Increased Revenue
              </dt>
              <dd class="mt-2 text-base leading-7 text-gray-600">
                Access a wider customer base and boost your sales through our platform.
              </dd>
            </div>
            <div class="relative pl-16">
              <div class="absolute left-0 top-0 flex h-10 w-10 items-center justify-center rounded-lg bg-indigo-600">
                <svg class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M18 18.72a9.094 9.094 0 003.741-.479 3 3 0 00-4.682-2.72m.94 3.198l.001.031c0 .225-.012.447-.037.666A11.944 11.944 0 0112 21c-2.17 0-4.207-.576-5.963-1.584A6.062 6.062 0 016 18.719m12 0a5.971 5.971 0 00-.941-3.197m0 0A5.995 5.995 0 0012 12.75a5.995 5.995 0 00-5.058 2.772m0 0a3 3 0 00-4.681 2.72 8.986 8.986 0 003.74.477m.94-3.197a5.971 5.971 0 00-.94 3.197M15 6.75a3 3 0 11-6 0 3 3 0 016 0zm6 3a2.25 2.25 0 11-4.5 0 2.25 2.25 0 014.5 0zm-13.5 0a2.25 2.25 0 11-4.5 0 2.25 2.25 0 014.5 0z" />
                </svg>
              </div>
              <dt class="text-lg font-semibold leading-7 text-gray-900">
                Community Support
              </dt>
              <dd class="mt-2 text-base leading-7 text-gray-600">
                Join a network of local businesses and share experiences and resources.
              </dd>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- CTA Section -->
    <div class="bg-white py-24 sm:py-32">
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div class="relative isolate overflow-hidden bg-gray-900 px-6 py-24 shadow-2xl sm:rounded-3xl sm:px-24">
          <h2 class="mx-auto max-w-2xl text-center text-3xl font-bold tracking-tight text-white sm:text-4xl">
            Ready to grow your business?
          </h2>
          <p class="mx-auto mt-6 max-w-xl text-center text-lg leading-8 text-gray-300">
            Join hundreds of local businesses already thriving on our platform.
            Get started today and reach more customers in your area.
          </p>
          <div class="mt-10 flex justify-center">
            <button class="rounded-md bg-white px-6 py-3 text-lg font-semibold text-gray-900 shadow-sm hover:bg-gray-100">
              Start Your Free Trial
            </button>
          </div>
        </div>
      </div>
    </div>

    <!-- Footer -->
    <footer class="bg-gray-900">
      <div class="mx-auto max-w-7xl px-6 py-12 md:flex md:items-center md:justify-between lg:px-8">
        <div class="mt-8 md:order-1 md:mt-0">
          <p class="text-center text-xs leading-5 text-gray-400">
            &copy; 2024 801 Collective. All rights reserved.
          </p>
        </div>
      </div>
    </footer>
  </div>
</template>

<script setup>
// Add any required Vue logic here
</script>

<style>
/* Add any custom styles here */
</style>