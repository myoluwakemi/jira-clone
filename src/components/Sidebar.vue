<template>
  <div>
    <div
      :class="[sideBarOpen ? 'show' : 'notShow']"
      class="fixed inset-0 bg-black opacity-50 lg:hidden side-bar_overlay"
    ></div>
    <div
      :class="[sideBarOpen ? 'sideBarOpen' : 'sideBarClose']"
      class="fixed inset-y-0 left-0 z-30 w-64 px-8 py-3 bg-gray-100 border-r overflow-auto lg:translate-x-0 lg:static lg:inset-auto"
    >
      <div class="flex justify-between items-center">
        <div class="rounded-xl h-9 w-9 bg-gray-700"></div>
        <button @click="$emit('toggle')" class="text-gray-600 lg:hidden">
          <i class="fas fa-times"></i>
        </button>
      </div>
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
  </div>
</template>

<script>
export default {
  name: "Sidebar",
  data: () => {
    return {};
  },
  props: {
    sideBarOpen: {
      type: Boolean,
      default: true,
    },
  },
};
</script>

<style scoped>
.show {
  display: block;
}
.notShow {
  display: none;
}
.sideBarOpen {
  transform: translateX(0);
  transition: 500ms ease-out;
}
.sideBarClose {
  transform: translateX(-100%);
  transition: 500ms ease-in;
}

@media (min-width: 1024px) {
  .side-bar_overlay {
    display: none;
  }
}
</style>
