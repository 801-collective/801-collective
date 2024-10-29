<template>
    <div class="card-header">
        <h2 class="card-title">Join the 801 Collective</h2>

      </div>
    <div class="shadow-md rounded-lg bg-white/50 backdrop-blur-sm w-full max-w-md">
      <div class="card-content">
        <div class="text-center text-indigo-600">
            Step {{ currentStep }} of {{ stepCount }}
        </div>
        <div class="progress-bar">
            <div class="progress-bar-fill" :style="{ width: `${((currentStep-1) / 2) * 100}%` }"></div>
        </div>
        <form @submit.prevent="handleSubmit">
          <!-- Step 1 -->
          <div v-if="currentStep === 1">
            <div class="mb-4">
              <label for="businessName" class="block font-medium text-gray-700 mb-1">
                Business Name
                <div>
                    <span class="text-sm text-gray-500">This will be your public business name</span>
                </div>
              </label>
              <input
                id="businessName"
                v-model="formData.businessName"
                type="text"
                class="input"
                required
              />
            </div>
            <div class="mb-4">
              <label for="email" class="block font-medium text-gray-700 mb-1">
                Email Address
                <div>
                    <span v-if="validEmail" class="text-sm text-gray-500">We'll never share your email with anyone else.</span>
                    <span v-else class="text-sm text-red-500">Please enter a valid email</span>
                </div>
              </label>
              <input
                id="email"
                v-model="formData.email"
                type="email"
                class="input"
                @input="validEmail = true"
                @blur="validEmail = validateEmail(formData.email)"
                required
              />
            </div>
            <div class="mb-6">
              <label for="password" class="block font-medium text-gray-700 mb-1">
                Password
                <div>
                    <span v-if="validPassword" class="text-sm text-gray-500">Must be at least 8 characters</span>
                    <span v-else class="text-sm text-red-500">Password must be at least 8 characters</span>
                </div>
              </label>

              <input
                id="password"
                v-model="formData.password"
                type="password"
                class="input"
                @input="validPassword = true"
                @blur="validPassword = validatePassword(formData.password)"
                required
              />
            </div>
            <button type="button" class="btn w-full" @click="verifyNext">
              Next
            </button>
          </div>

          <!-- Step 2 -->
          <div v-if="currentStep === 2">
            <div class="mb-4">
              <label for="street" class="block font-medium text-gray-700 mb-1">
                Street Address
              </label>
              <input
                id="street"
                v-model="formData.address.street"
                type="text"
                class="input"
                required
              />
            </div>
            <div class="mb-4">
              <label for="city" class="block font-medium text-gray-700 mb-1">
                City
              </label>
              <input
                id="city"
                v-model="formData.address.city"
                type="text"
                class="input"
                required
              />
            </div>
            <div class="mb-4">
              <label for="state" class="block font-medium text-gray-700 mb-1">
                State
              </label>
              <input
                id="state"
                v-model="formData.address.state"
                type="text"
                class="input"
                required
              />
            </div>
            <div class="mb-6">
              <label for="zip" class="block font-medium text-gray-700 mb-1">
                ZIP Code
              </label>
              <input
                id="zip"
                v-model="formData.address.zip"
                type="text"
                class="input"
                required
              />
            </div>
            <div class="flex justify-between">
              <button type="button" class="btn w-1/2 mr-2" @click="currentStep = 1">
                Back
              </button>
              <button type="submit" class="btn w-1/2 ml-2">
                Sign Up
              </button>
            </div>
          </div>
        </form>
      </div>
    </div>
  </template>

<script setup>
import { ref } from 'vue';

const stepCount = 2;
const currentStep = ref(1);
const formData = ref({
businessName: '',
email: '',
password: '',
address: {
    street: '',
    city: '',
    state: '',
    zip: '',
},
});

const validEmail = ref(true);
const validPassword = ref(true);

function validateEmail(email) {
    if (/^\w+([\.-]?\w+)*@\w+([\.-]?\w+)*(\.\w{2,3})+$/.test(email)) {
        return (true)
    } else {
        return (false)
    }
}

function validatePassword(password) {
    if (password.length >= 8) {
        return true;
    } else {
        return false;
    }
}


function verifyNext() {
// check if the form is valid before moving to the next step
if (currentStep.value === 1) {
    if (!formData.value.businessName || !formData.value.email || !formData.value.password) {
    alert('Please fill out all fields');
    }
    if (!validatePassword(formData.value.password)) {
    validPassword.value = false;
    }
    if (!validateEmail(formData.value.email)) {
    validEmail.value = false;
    }
    if(formData.value.businessName && formData.value.email && formData.value.password && formData.value.password.length >= 8 && validateEmail(formData.value.email)) {
    currentStep.value++;
    }
} else if (currentStep.value === 2) {
    if (!formData.value.address.street || !formData.value.address.city || !formData.value.address.state || !formData.value.address.zip) {
    alert('Please fill out all fields');
    return;
    }
    else {
        handleSubmit();
    }
}
}

function handleSubmit() {
// Add your sign up logic here
console.log('Submitting form:', formData.value);
}
</script>

  <style>
  .card {
    @apply bg-white shadow-md rounded-lg;
  }

  .card-header {
    @apply text-gray-900 rounded-t-lg px-2 py-4 w-full max-w-md mb-1;
  }

  .card-title {
    @apply text-3xl font-bold text-center;
  }

  .progress-bar {
    @apply w-full bg-gray-300 rounded-full h-1 mt-2 mb-4;
    }

    .progress-bar-fill {
    @apply bg-green-500 h-full rounded-full transition-all duration-300 ease-in-out;
    }

  .card-content {
    @apply p-6;
  }

  .input {
    @apply block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500;
  }

  .btn {
    @apply inline-flex justify-center py-2 px-4 border border-transparent shadow-sm text-sm font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500;
  }
  </style>