<template>
  <header>
    <div class="px-6">
      <div
        class="flex justify-between items-center border-b border-gray-200 py-3"
      >
        <div class="flex-1 flex">
          <button @click="$emit('toggle')" class="text-gray-600 lg:hidden">
            <svg class="h6 w-6" viewBox="0 0 24 24" fill="none">
              <path
                d="M4 6h16M4 12h16M4 18h7"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
              />
            </svg>
          </button>
          <div class="ml-4 relative lg:ml-0">
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
        <div class="items-center sm:flex">
          <h2 class="text-2xl font-semibold text-gray-900">All issues</h2>
          <div class="mt-1 flex items-center sm:ml-6 sm:mt-0">
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
          <span class="hidden sm:inline-flex p-1 border bg-gray-200 rounded-md">
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
    </div>
    <div class="flex px-4 p-1 border-b bg-gray-200 lg:hidden">
      <button
        class="w-1/2 inline-flex justify-center px-2 py-1 rounded leading-none"
      >
        <i class="fas fa-align-justify h-6 w-6 text-gray-600"></i>
        <span class="ml-2 text-sm text-gray-900 font-medium">list</span>
      </button>
      <button
        class="w-1/2 inline-flex justify-center px-2 py-1 bg-white rounded leading-none shadow"
      >
        <i class="fas fa-columns h-6 w-6 text-gray-600"></i>
        <span class="ml-2 text-sm text-gray-900 font-medium">Board</span>
      </button>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped></style>
