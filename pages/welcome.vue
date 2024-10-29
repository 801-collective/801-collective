<!-- App.vue -->
<template>
    <div class="min-h-screen bg-gradient-to-b from-indigo-100 to-white">


      <!-- Hero Section -->
      <section class="pt-32 pb-32 bg-gradient-to-b from-indigo-200 to-white">
        <div class="mt-12 mb-12 h-80 w-80 mx-auto flex justify-center items-center absolute top-1/2 -translate-y-1/2 left-0 right-0">
          <img class="h-fill w-auto" src="../public/images/iphone.png" alt="">
        </div>
        <div class="shadow-md rounded-lg p-10 bg-white/50 backdrop-blur-sm w-full max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
          <div class="text-center">
            <h2 class="text-4xl md:text-6xl font-bold text-gray-900 mb-6">
              Grow Your Local Business Online
            </h2>
            <p class="text-xl text-gray-600 mb-8 max-w-3xl mx-auto">
              Join hundreds of local businesses reaching new customers through the 801 Collective marketplace. We help you connect with customers who value shopping local.
            </p>
            <div class="flex flex-col sm:flex-row justify-center gap-4">
              <button class="bg-indigo-600 text-white px-8 py-4 rounded-full text-lg hover:bg-indigo-700 transition">
                Start Selling Today
              </button>
              <button class="border-2 border-indigo-600 text-indigo-600 px-8 py-4 rounded-full text-lg hover:bg-indigo-100 transition">
                Learn More
              </button>
            </div>
          </div>
        </div>
      </section>

      <!-- Features Section -->
      <section id="features" class="py-20 bg-gradient-to-b from-white to-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <h3 class="text-3xl font-bold text-center mb-16">Everything You Need to Succeed</h3>
          <div class="grid md:grid-cols-3 gap-8">
            <div class="text-center p-6">
              <div class="w-16 h-16 bg-indigo-100 rounded-full flex items-center justify-center mx-auto mb-4">
                <svg class="w-8 h-8 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
                </svg>
              </div>
              <h4 class="text-xl font-semibold mb-2">Quick Setup</h4>
              <p class="text-gray-600">Create your store profile and start selling in minutes with our easy-to-use platform.</p>
            </div>
            <div class="text-center p-6">
              <div class="w-16 h-16 bg-indigo-100 rounded-full flex items-center justify-center mx-auto mb-4">
                <svg class="w-8 h-8 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6v6m0 0v6m0-6h6m-6 0H6" />
                </svg>
              </div>
              <h4 class="text-xl font-semibold mb-2">Local Exposure</h4>
              <p class="text-gray-600">Connect with customers in your area who are specifically looking for local businesses.</p>
            </div>
            <div class="text-center p-6">
              <div class="w-16 h-16 bg-indigo-100 rounded-full flex items-center justify-center mx-auto mb-4">
                <svg class="w-8 h-8 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z" />
                </svg>
              </div>
              <h4 class="text-xl font-semibold mb-2">Growth Analytics</h4>
              <p class="text-gray-600">Track your performance and understand your customers with detailed analytics.</p>
            </div>
          </div>
        </div>
      </section>

      <!-- Benefits Section -->
      <section id="benefits" class="py-20 bg-gradient-to-b from-gray-50 to-indigo-50 flex justify-center">
        <div class="max-w-7xl sm:px-6 lg:px-8 bg-gray-900 text-white p-6 rounded-lg m-4">
          <div class="grid md:grid-cols-2 gap-12 items-center">
            <div>
              <h3 class="text-3xl font-bold mb-6">Why Join 801 Collective?</h3>
              <ul class="space-y-4">
                <li class="flex items-start">
                  <svg class="w-6 h-6 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
                  </svg>
                  <span>Reach thousands of local customers actively looking to support small businesses</span>
                </li>
                <li class="flex items-start">
                  <svg class="w-6 h-6 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
                  </svg>
                  <span>No technical expertise required - we handle the technology so you can focus on your business</span>
                </li>
                <li class="flex items-start">
                  <svg class="w-6 h-6 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
                  </svg>
                  <span>Flexible pricing plans that grow with your business</span>
                </li>
              </ul>
            </div>
            <div class="bg-white p-8 rounded-lg shadow-lg">
              <form class="space-y-4">
                <div>
                  <label class="block text-sm font-medium text-gray-700">Business Name</label>
                  <input type="text" class="mt-1 text-black block w-full rounded-md border-gray-300 shadow-sm focus:border-blue-500 focus:ring-blue-500" />
                </div>
                <div>
                  <label class="block text-sm font-medium text-gray-700">Email Address</label>
                  <input type="email" class="mt-1 text-black block w-full rounded-md border-gray-300 shadow-sm focus:border-blue-500 focus:ring-blue-500" />
                </div>
                <div>
                  <label class="block text-sm font-medium text-gray-700">Business Type</label>
                  <select class="mt-1 block w-full text-black rounded-md border-gray-300 shadow-sm focus:border-blue-500 focus:ring-blue-500">
                    <option>Retail</option>
                    <option>Food & Beverage</option>
                    <option>Services</option>
                    <option>Other</option>
                  </select>
                </div>
                <button class="w-full bg-indigo-600 text-white px-6 py-3 rounded-md hover:bg-indigo-700 transition">
                  Join the Collective
                </button>
              </form>
            </div>
          </div>
        </div>
      </section>

      <!-- Testimonials Section -->
      <section id="testimonials" class="py-20 bg-indigo-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <h3 class="text-3xl font-bold text-center mb-16">Success Stories</h3>
          <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
            <div class="bg-white p-6 rounded-lg shadow-md">
              <div class="flex items-center mb-4">
                <div class="w-12 h-12 bg-indigo-100 rounded-full"></div>
                <div class="ml-4">
                  <h4 class="font-semibold">Sarah Johnson</h4>
                  <p class="text-sm text-gray-600">Local Bakery Owner</p>
                </div>
              </div>
              <p class="text-gray-600">"Since joining 801 Collective, our customer base has grown by 40%. The platform made it easy to showcase our products and connect with local customers."</p>
            </div>
            <div class="bg-white p-6 rounded-lg shadow-md">
              <div class="flex items-center mb-4">
                <div class="w-12 h-12 bg-indigo-100 rounded-full"></div>
                <div class="ml-4">
                  <h4 class="font-semibold">Mike Thompson</h4>
                  <p class="text-sm text-gray-600">Craft Store Owner</p>
                </div>
              </div>
              <p class="text-gray-600">"The analytics tools helped us understand our customers better. We've been able to optimize our inventory and increase sales significantly."</p>
            </div>
            <div class="bg-white p-6 rounded-lg shadow-md">
              <div class="flex items-center mb-4">
                <div class="w-12 h-12 bg-indigo-100 rounded-full"></div>
                <div class="ml-4">
                  <h4 class="font-semibold">Lisa Chen</h4>
                  <p class="text-sm text-gray-600">Boutique Owner</p>
                </div>
              </div>
              <p class="text-gray-600">"The support from 801 Collective has been amazing. They truly care about helping small businesses succeed in the digital space."</p>
            </div>
          </div>
        </div>
      </section>

    </div>
</template>