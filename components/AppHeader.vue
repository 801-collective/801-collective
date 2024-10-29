<template>
<!-- Navigation -->
  <nav class="fixed w-full bg-white/90 backdrop-blur-sm shadow-sm z-50">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-16">
        <NuxtLink to="/welcome" class="flex-shrink-0">
          <h1 class="text-2xl font-bold text-indigo-600">801 Collective</h1>
        </NuxtLink>
        <div class="hidden md:block">
          <div class="flex items-center space-x-8">
            <NuxtLink to="/welcome#features" class="text-gray-600 hover:text-indigo-600">Features</NuxtLink>
            <NuxtLink to="/welcome#benefits" class="text-gray-600 hover:text-indigo-600">Benefits</NuxtLink>
            <NuxtLink to="/welcome#testimonials" class="text-gray-600 hover:text-indigo-600">Success Stories</NuxtLink>
            <button class="bg-indigo-600 text-white px-6 py-2 rounded-full hover:bg-indigo-700 transition">
              <NuxtLink to="/signup">Sign Up Now</NuxtLink>
            </button>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>