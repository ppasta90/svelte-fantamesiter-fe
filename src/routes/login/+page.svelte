<script lang="ts">
  let email = '';
  let password = '';

  function handleSubmit() {
    // TODO: Implement login logic
    console.log('Login submitted:', { email, password });
  }
</script>

<div class="w-full max-w-2xl mx-auto p-6 bg-white rounded-lg shadow-md">
  <h1 class="text-2xl font-bold mb-2 text-center">Log In to Your Account</h1>
  <p class="text-gray-600 mb-6 text-center">Welcome back to FantaMeister!</p>

  <form on:submit|preventDefault={handleSubmit}>
    <div class="mb-4">
      <label for="email" class="block text-sm font-medium text-gray-700">Email</label>
      <input
        type="email"
        id="email"
        bind:value={email}
        required
        class="mt-1 block w-full rounded-md border-gray-300 shadow-sm focus:border-indigo-300 focus:ring focus:ring-indigo-200 focus:ring-opacity-50"
      />
    </div>

    <div class="mb-6">
      <label for="password" class="block text-sm font-medium text-gray-700">Password</label>
      <input
        type="password"
        id="password"
        bind:value={password}
        required
        class="mt-1 block w-full rounded-md border-gray-300 shadow-sm focus:border-indigo-300 focus:ring focus:ring-indigo-200 focus:ring-opacity-50"
      />
    </div>

    <button
      type="submit"
      class="w-full py-2 px-4 border border-transparent rounded-md shadow-sm text-sm font-medium text-white bg-indigo-600 hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
    >
      Log In
    </button>
  </form>

  <p class="mt-4 text-center text-sm text-gray-600">
    Don't have an account? 
    <a href="/register" class="font-medium text-indigo-600 hover:text-indigo-500">
      Register here
    </a>
  </p>
</div>
