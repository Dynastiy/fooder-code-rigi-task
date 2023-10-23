<template>
  <div class="">
    <app-header :menus="menus" />
    <slot />
    <app-footer class="tw-mt-6"/>
  </div>
</template>

<script>
import AppHeader from "@/components/Navigation/AppHeader.vue";
import AppFooter from "@/components/Navigation/AppFooter.vue";
export default {
  components: { AppHeader, AppFooter },
  name: "AppHomeLayout",

  data(){
    return {
      menus: [
        {
          title: "home",
          href: "/",
          parent: "home",
          id: "home"
        },
        {
          title: "about us",
          href: "#about-us",
          parent: "about-us",
          id: "about-us"
        },
        {
          title: "contact us",
          href: "#contact-us",
          parent: "contact-us",
          id: "contact-us"
        }
      ]
    }
  }
};
</script>
