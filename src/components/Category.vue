<script setup>
const props = defineProps({

    category_title: {
        type: String, 
        default: ""
    }
})

</script>

<template>
    <div class="category bg-success text-white p-3 my-2 rounded-3" 
        role="button"
        :category_title = "category_title"
        @click="$emit('selected_category', category_title)"
    >
    <h4 class="mx-5">{{ category_title }}</h4>     
    </div>
</template>

