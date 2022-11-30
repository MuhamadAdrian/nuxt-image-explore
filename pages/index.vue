<script lang="ts" setup>
const tags = ref([
  "sports",
  "adventure",
  "movies",
  "health",
  "education",
  "polite",
  "sosial",
  "event",
]);

const highlightedPost = ref([
  {
    id: 1,
    image: "",
    title: "Blog Title 1",
    description: `dolor sit amet consectetur adipisicing elit. Animi unde maiores
          repellat dignissimos doloremque, rem sint quibusdam corporis, quae
          quisquam neque exercitationem quasi tempore, culpa nostrum rerum minus
          aut provident!`,
  },
  {
    id: 2,
    image: "",
    title: "Blog Title 2",
    description: `dolor sit amet consectetur adipisicing elit. Animi unde maiores
          repellat dignissimos doloremque, rem sint quibusdam corporis, quae
          quisquam neque exercitationem quasi tempore, culpa nostrum rerum minus
          aut provident!`,
  },
  {
    id: 3,
    image: "",
    title: "Blog Title 3",
    description: `dolor sit amet consectetur adipisicing elit. Animi unde maiores
          repellat dignissimos doloremque, rem sint quibusdam corporis, quae
          quisquam neque exercitationem quasi tempore, culpa nostrum rerum minus
          aut provident!`,
  },
]);
</script>

<template>
  <div>
    <section class="py-20 text-gray-200">
      <div class="container px-10 mx-auto">
        <h1 class="text-center max-w-lg mx-auto text-2xl font-semibold mt-10">
          Lorem ipsum dolor sit amet consectetur adipisicing elit Lorem ipsum
        </h1>
        <div class="flex items-center flex-wrap justify-center mt-10 gap-3">
          <div
            v-for="(tag, index) in tags"
            :key="index"
            class="bg-indigo-700 px-3 py-1 rounded-md cursor-pointer hover:bg-indigo-800 transition-colors"
          >
            #{{ tag }}
          </div>
        </div>
        <div class="grid grid-cols-3 gap-4 mt-10">
          <div
            v-for="post in highlightedPost"
            :key="post.id"
            class="bg-gray-800 p-4 rounded-md"
          >
            <img :src="post.image" :alt="post.title" />
            <h2 class="font-semibold text-lg mt-3">{{ post.title }}</h2>
            <p class="mt-5 truncate block">
              {{ post.description }}
            </p>
            <button
              class="bg-indigo-600 hover:bg-indigo-700 transition-colors block w-full mt-5 px-4 py-3 rounded-md"
            >
              See Detail
            </button>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>
