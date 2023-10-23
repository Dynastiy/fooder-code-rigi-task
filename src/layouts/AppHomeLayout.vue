<template>
  <div class="">
    <app-header class="tw-sticky tw-top-0 tw-z-10" :menus="menus" @toggleDrawer="toggleDrawer"/>
    <slot />
    <app-footer class="tw-mt-6"/>

    <mobile-drawer @close="toggleDrawer" :menu="menus"  :drawer="drawer"/>
  </div>
</template>

<script>
import AppHeader from "@/components/Navigation/AppHeader.vue";
import AppFooter from "@/components/Navigation/AppFooter.vue";
import MobileDrawer from "@/components/Navigation/MobileDrawer.vue"
export default {
  components: { AppHeader, AppFooter, MobileDrawer },
  name: "AppHomeLayout",

  data(){
    return {
      menus: [
        {
          title: "home",
          href: "/",
          parent: "home",
          id: "home",
          icon: "iconoir:home"
        },
        {
          title: "about us",
          href: "#about-us",
          parent: "about-us",
          id: "about-us",
          icon: "mdi:about-circle-outline"
        },
        {
          title: "contact us",
          href: "#contact-us",
          parent: "contact-us",
          id: "contact-us",
          icon: "system-uicons:message"
        }
      ],
      drawer: false
    }
  },

  methods: {
    toggleDrawer(){
      this.drawer = !this.drawer
    },
  },
};
</script>
