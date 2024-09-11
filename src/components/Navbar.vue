<script setup>
import { ref, onMounted, computed, watch } from "vue";
import Category from "./Category.vue";
const categories = ref([
  { id: 1, title: "House" },
  { id: 2, title: "Office" },
  { id: 3, title: "Store" },
]);
function Show(cat) {
    console.log(cat)
}
</script>

<template>
    <section class="position-fixed">
      <Category
        v-for="category in categories"
        :category_title="category.title"
        :key="category.id"
        @selected_category="Show"
        >
      </Category>
    </section>
</template>
