<template>
  <div class="h-screen flex">
    <!--side nav--->
    <slot name="sidebar"> </slot>

    <!--main-content--->
    <div class="flex-1 min-w-0 flex flex-col bg-white">
      <div class="flex-shrink-0 flex-col border-b-2 border-gray-200">
        <slot name="main-header"></slot>
      </div>
      <div class="flex-1 overflow-auto">
        <slot name="kanban-area"> </slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "DashboardLayout",
};
</script>

<style scoped></style>
