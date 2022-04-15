<template>
  <div>
    <SidebarVue />
    <DashboardVue />
  </div>
</template>
<script>
import DashboardVue from "../../components/admin/Dashboard.vue";
import SidebarVue from "../../components/admin/Sidebar.vue";

export default {
  name: "DashboardPage",
  head(){
  return{
   title:'Dashboard',
  }
  },
  comp
  components: {
    SidebarVue,
    DashboardVue,
  },
};
</script>
<style>
</style>