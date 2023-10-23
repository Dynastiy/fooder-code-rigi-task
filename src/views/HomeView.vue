<template>
  <div class="home">
    <!-- App hero Section  -->
    <div class="hero-section tw-flex tw-items-center tw-py-5">
      <div class="lg:tw-px-16 md:tw-px-12 tw-px-6">
        <h1
          class="tw-text-white tw-text-[40px] lg:tw-text-[60px] md:tw-text-[60px] lg:tw-tracking-widest md:tw-tracking-widest tw-font-bold lg:tw-w-5/12 md:tw-w-5/12"
        >
          Lorem ipsum dolor elit
        </h1>
        <p class="tw-text-sm tw-text-gray-400 lg:tw-w-5/12 md:tw-w-5/12">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quos
          molestias, mollitia tempora suscipit quasi aut voluptatem magni
          accusamus nostrum et beatae a laudantium commodi iste obcaecati
          numquam iusto enim? Tempora? mollitia tempora suscipit quasi aut
          voluptatem magni accusamus nostrum et beatae mollitia tempora suscipit
          quasi aut voluptatem magni accusamus nostrum et beatae
        </p>
        <button class="main-btn main-btn-primary">place order</button>
      </div>
    </div>

    <!-- Menus -->
    <section class="tw-mt-12 lg:tw-px-16 md:tw-px-12 tw-px-6">
      <!-- Pagination for product list  -->
      <div>
        <product-list-pagination />
      </div>
      <div
        class="tw-grid lg:tw-grid-cols-4 md:tw-grid-cols-2 tw-grid-cols-1 tw-gap-5"
      >
        <!-- Component for menus - listing dishes and their prices  -->
        <dishes-cards v-for="item in 8" :key="item" />
      </div>
    </section>

    <section class="tw-mt-12" id="about-us">
        <about-us />
    </section>
  </div>
</template>

<script>
import DishesCards from "@/components/Cards/DishesCards.vue";
import ProductListPagination from '@/components/Navigation/ProductListPagination.vue';
import AboutUs from '@/components/Sections/AboutUs.vue';
export default {
  name: "HomeView",
  components: { DishesCards, ProductListPagination, AboutUs },
};
</script>

<style>
.hero-section {
  background: url("https://ik.imagekit.io/awwybhhmo/satellite_images/thai/beyondmenu/hero/12.jpg?tr=w-3840,q-50");
  min-height: 500px;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
}
</style>
