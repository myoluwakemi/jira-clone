<template>
  <DashboardLayout>
    <template #sidebar>
      <Sidebar @toggle="sideBarOpen = false" :side-bar-open="sideBarOpen"/>
    </template>
    <template #main-header>
      <Header @toggle="sideBarOpen = true" />
    </template>
    <template #kanban-area>
      <KanbanView />
    </template>
  </DashboardLayout>
</template>

<script>
import DashboardLayout from "../Layouts/DashboardLayout";
import Sidebar from "../components/Sidebar";
import Header from "../components/Header";
import KanbanView from "../components/KanbanView";
export default {
  name: "Dashboard",
  components: { KanbanView, Header, Sidebar, DashboardLayout },
  data: () => {
    return {
      sideBarOpen: true,
    };
  },
};
</script>

<style scoped></style>
