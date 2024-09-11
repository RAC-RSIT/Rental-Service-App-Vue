<script setup>
import { ref, onMounted, computed, watch } from "vue";
import SingleProperty from "./SingleProperty.vue";
import data from "@/assets/data";

</script>

<template>
    <div class="property_list row d-flex justify-content-between" >
        <SingleProperty
            v-for="property in data.property_list"
            :key="property.id"
            :title="property.title"
            :desc="property.desc"
            :rent="property.rent"
            :category="property.category"
            :garage="property.garage"
            @click="console.log(`${property.title} found`)" 
        ></SingleProperty>
    </div>
</template>

