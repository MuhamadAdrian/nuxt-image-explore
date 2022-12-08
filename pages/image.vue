<script setup lang="ts"></script>
<template>
  <section class="py-20 text-gray-200">
    <div class="container px-10 mx-auto">
      <div>
        With Image Tag:
        <img
          src="/images/blog-1.jpg"
          width="4501"
          height="2501"
          alt="Blog Image"
        />
      </div>
      <div class="mt-20">
        With NuxtImage Tag:
        <nuxt-img
          src="/images/blog-1.jpg"
          width="4501"
          height="2501"
          alt="Blog Image"
        />
      </div>
      <div class="mt-20">
        With NuxtPicture Tag:
        <nuxt-picture
          src="/images/blog-1.jpg"
          width="4501"
          height="2501"
          alt="Blog Image"
        />
      </div>
    </div>
  </section>
</template>
