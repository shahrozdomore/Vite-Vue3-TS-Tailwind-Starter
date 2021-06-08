<template>
  <div>
    <header class="bg-white shadow" v-if="$route.meta.title">
      <div class="inline-flex rounded-md shadow">
        <router-link to="/" class="">Home</router-link> |
        <router-link to="/about" class="">About</router-link>
      </div>
      <div class="max-w-7xl mx-auto py-6 px-4 sm:px-6 lg:px-8">
        <h1 class="text-3xl font-bold leading-tight text-gray-900">{{ $route.meta.title }}</h1>
      </div>
    </header>
    <main>
      <router-view />
    </main>
  </div>
</template>
