<template>
  <div>
    <q-layout view="hHr LpR lFf">
      <q-layout-header reveal v-model="header">
        <q-toolbar color="secondary">
          <q-btn flat round dense icon="menu" @click="menuVisible = !menuVisible"/>
          <q-toolbar-title>首页</q-toolbar-title>
        </q-toolbar>
      </q-layout-header>
      <q-layout-drawer side="left" v-model="menuVisible">
        <SideMenu />
      </q-layout-drawer>
    </q-layout>
  </div>
</template>

<script>
import SideMenu from './SideMenu.vue';
export default {
    components: {
        SideMenu
    },
  data() {
    return {
      menuVisible: false,
      color: 'red',
      header: "",
      simple: [
        {
          label: "Satisfied customers",
          children: [
            {
              label: "Good food",
              children: [
                { label: "Quality ingredients" },
                { label: "Good recipe" }
              ]
            },
            {
              label: "Pleasant surroundings",
              children: [
                { label: "Happy atmosphere" },
                { label: "Good table presentation" },
                { label: "Pleasing decor" }
              ]
            }
          ]
        },
        {
          label: "Satisfied customers",
          children: [
            {
              label: "Good food",
              children: [
                { label: "Quality ingredients" },
                { label: "Good recipe" }
              ]
            },
            {
              label: "Pleasant surroundings",
              children: [
                { label: "Happy atmosphere" },
                { label: "Good table presentation" },
                { label: "Pleasing decor" }
              ]
            }
          ]
        }
      ]
    };
  }
};
</script>

<style scoped>
</style>