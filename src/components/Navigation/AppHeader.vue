<template>
  <div class="tw-bg-white tw-px-8 tw-py-6 tw-shadow-xl">
    <div class="tw-flex tw-justify-between">
      <div class="tw-flex tw-items-center tw-gap-12">
        <span class="tw-font-bold">fooder</span>

        <ul
          class="lg:tw-flex md:tw-flex tw-hidden tw-mb-0 tw-gap-4 tw-items-center"
        >
          <li v-for="(item, idx) in menus" :key="idx">
            <a
              class="tw-text-black tw-text-sm tw-no-underline hover:tw-text-primary tw-font-medium"
              :href="item.href"
            >
              {{ item.title }}</a
            >
          </li>
        </ul>
      </div>
      <div class="lg:tw-flex md:tw-flex tw-hidden tw-gap-3 tw-items-center">
        <a href="#" class="tw-text-black">
          <i-icon
            icon="eva:facebook-fill"
            class="tw-text-blue-700"
            width="18px"
          />
        </a>
        <a href="#" class="tw-text-black">
          <i-icon icon="bi:instagram" width="18px" class="tw-text-red-400" />
        </a>
        <a href="#" class="tw-text-black">
          <i-icon
            icon="teenyicons:twitter-outline"
            class="tw-text-blue-400"
            width="18px"
          />
        </a>
      </div>

      <span class="tw-block lg:tw-hidden md:tw-hidden" role="button" @click="$emit('toggleDrawer')">
          <i-icon icon="ri:menu-fill" width="24px" />
        </span>
    </div>
  </div>
</template>

<script>
export default {
  // Resuable props for the menu items imported from the app home layout
  props: {
    menus: {
      type: Array,
      defualt: () => [],
    },
  },
};
</script>

<style></style>
