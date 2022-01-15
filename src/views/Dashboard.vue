<template>
  <div class="h-screen flex">
    <!--    side bar-->
    <div class="w-64 px-8 py-3 bg-gray-100 border-r">
      <div class="rounded-xl h-9 w-9 bg-gray-700"></div>
      <nav class="mt-8">
        <h3
          class="text-xs font-semibold text-gray-600 uppercase tracking-wider"
        >
          Issues
        </h3>
        <div class="mt-2 -mx-3">
          <a
            href="#"
            class="flex justify-between items-center px-3 py-2 bg-gray-200 rounded-lg"
          >
            <span class="font-medium text-gray-900">All</span>
            <span class="text-xs font-semibold text-grey-700">36</span>
          </a>
          <a
            href="#"
            class="flex justify-between items-center px-3 py-2 rounded-lg"
          >
            <span class="font-medium text-gray-900">Assigned to me</span>
            <span class="text-xs font-semibold text-grey-700">2</span>
          </a>
          <a
            href="#"
            class="flex justify-between items-center px-3 py-2 rounded-lg"
          >
            <span class="font-medium text-gray-900">Created by me</span>
            <span class="text-xs font-semibold text-grey-700">1</span>
          </a>
          <a
            href="#"
            class="flex justify-between items-center px-3 py-2 rounded-lg"
          >
            <span class="font-medium text-gray-900">Archived</span>
          </a>
        </div>
        <h3
          class="mt-8 text-xs font-semibold text-gray-600 uppercase tracking-wider"
        >
          Tags
        </h3>
        <div class="mt-2 -mx-3">
          <a
            href="#"
            class="flex justify-between items-center px-3 py-2 rounded-lg"
          >
            <span class="font-medium text-gray-900">Bugs</span>
          </a>
          <a
            href="#"
            class="flex justify-between items-center px-3 py-2 rounded-lg"
          >
            <span class="font-medium text-gray-900">Feature Request</span>
          </a>
          <a
            href="#"
            class="flex justify-between items-center px-3 py-2 rounded-lg"
          >
            <span class="font-medium text-gray-900">Marketing</span>
          </a>
          <a
            href="#"
            class="flex justify-between items-center px-3 py-2 rounded-lg"
          >
            <span class="font-medium text-gray-900">v2.0</span>
          </a>
          <a
            href="#"
            class="flex justify-between items-center px-3 py-2 rounded-lg"
          >
            <span class="font-medium text-gray-900">Enhancement</span>
          </a>
          <a
            href="#"
            class="flex justify-between items-center px-3 py-2 rounded-lg"
          >
            <span class="font-medium text-gray-900">Design</span>
          </a>
        </div>
        <button class="mt-2 -ml-1 text-xs font-medium text-gray-600">
          <i class="fas fa-plus h-5 w-5 text-gray-500"></i>
          New Project
        </button>
      </nav>
    </div>
    <!--    main area-->
    <div class="flex-1 min-w-0 bg-white">
      <!--      top section-->
      <div class="border-b-2 border-gray-200">
        <header class="px-6">
          <div
            class="flex justify-between items-center border-b border-gray-200 py-3"
          >
            <div>
              <div class="relative">
                <span class="absolute bottom-0 left-0 pl-2 flex items-center"
                  ><i class="fas fa-search h-6 w-6 text-gray-600"></i
                ></span>
                <input
                  class="block w-full rounded-md border-solid border-2 border-gray-400 pl-10 pr-4 py-2 text-sm text-gray-900 placeholder-gray-600"
                  type="search"
                  placeholder="search"
                />
              </div>
            </div>
            <div class="flex items-center">
              <button>
                <i class="far fa-bell"></i>
              </button>
              <button class="ml-6">
                <img
                  class="h-9 w-9 rounded-full object-cover"
                  src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                  alt="photo"
                />
              </button>
            </div>
          </div>
          <div class="flex items-center justify-between py-2">
            <div class="flex items-center">
              <h2 class="text-2xl font-semibold text-gray-900">All issues</h2>
              <div class="ml-6 flex items-center">
                <span class="border-2 rounded-full border-white">
                  <img
                    class="h-6 w-6 rounded-full object-cover"
                    src="https://images.unsplash.com/photo-1531427186611-ecfd6d936c79?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=facearea&facepad=2.2&w=144&h=144&q=80"
                    alt="person-1"
                  />
                </span>
                <span class="-ml-2 border-2 rounded-full border-white">
                  <img
                    class="h-6 w-6 rounded-full object-cover"
                    src="https://images.unsplash.com/photo-1506697084665-7f7d652308af?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=facearea&facepad=2&w=144&h=144&q=80"
                    alt="person-2"
                  />
                </span>
                <span class="-ml-2 rounded-full border-white">
                  <img
                    class="h-6 w-6 rounded-full object-cover"
                    src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                    alt="photo"
                  />
                </span>
                <span class="-ml-2 border-2 rounded-full border-white">
                  <img
                    class="h-6 w-6 rounded-full object-cover"
                    src="https://images.unsplash.com/photo-1529111290557-82f6d5c6cf85?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=facearea&facepad=2&w=144&h=144&q=80"
                    alt="person3"
                  />
                </span>
              </div>
            </div>
            <div class="flex">
              <span class="inline-flex p-1 border bg-gray-200 rounded-md">
                <button class="px-2 py-1 rounded">
                  <i class="fas fa-align-justify h-6 w-6 text-gray-600"></i>
                </button>
                <button class="px-2 py-1 bg-white rounded shadow">
                  <i class="fas fa-columns h-6 w-6 text-gray-600"></i>
                </button>
              </span>
              <button
                class="ml-5 px-4 py-2 text-xs font-medium text-white bg-gray-900 rounded-md hover:bg-gray-700"
              >
                <i class="fas fa-plus h-5 w-5 text-gray-500"></i>
                New Issue
              </button>
            </div>
          </div>
        </header>
      </div>
      <div class="">
        <main></main>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Dashboard",
};
</script>

<style scoped></style>
