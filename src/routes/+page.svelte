<script lang="ts">
  import { goto } from '$app/navigation';

  function navigateToLogin() {
    goto('/login');
  }

  function navigateToRegister() {
    goto('/register');
  }
</script>

<div class="max-w-2xl mx-auto p-8 bg-white rounded-lg shadow-md text-center">
  <h1 class="text-4xl font-bold mb-4 text-indigo-600">FantaMeister</h1>
  <p class="text-xl text-gray-600 mb-8">
    Welcome to FantaMeister, the ultimate fantasy football experience. Create your dream team, compete with friends, and prove you're the true FantaMeister!
  </p>

  <div class="space-y-4">
    <button
      on:click={navigateToLogin}
      class="w-full py-2 px-4 border border-transparent rounded-md shadow-sm text-sm font-medium text-white bg-indigo-600 hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
    >
      Login
    </button>
    <button
      on:click={navigateToRegister}
      class="w-full py-2 px-4 border border-indigo-600 rounded-md shadow-sm text-sm font-medium text-indigo-600 bg-white hover:bg-indigo-50 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
    >
      Register
    </button>
  </div>
</div>
