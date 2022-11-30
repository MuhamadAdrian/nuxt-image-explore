<template>
  <header class="bg-gray-800 text-white fixed top-0 left-0 w-full shadow-md">
    <div class="container mx-auto px-10 py-5">
      <div class="flex items-center justify-between">
        <div class="uppercase font-bold text-lg">Logo</div>
        <ul class="flex items-center gap-x-5 text-indigo-300 no-underline">
          <li>
            <NuxtLink
              active-class="font-bold text-indigo-500 py-3 px-5 bg-indigo-500 bg-opacity-10 rounded-xl"
              to="#"
              >Home</NuxtLink
            >
          </li>
          <li>
            <NuxtLink
              active-class="font-bold text-indigo-500 py-3 px-5 bg-indigo-500 bg-opacity-10 rounded-xl"
              to="/blog"
              >Blog</NuxtLink
            >
          </li>
          <li>
            <NuxtLink
              active-class="font-bold text-indigo-500 py-3 px-5 bg-indigo-500 bg-opacity-10 rounded-xl"
              to="/about"
              >About</NuxtLink
            >
          </li>
          <li>
            <NuxtLink
              active-class="font-bold text-indigo-500 py-3 px-5 bg-indigo-500 bg-opacity-10 rounded-xl"
              to="/project"
              >Project</NuxtLink
            >
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>
