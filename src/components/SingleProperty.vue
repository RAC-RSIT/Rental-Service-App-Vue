<script setup>
const props = defineProps({
    title: {
        type: String, 
        default: ""
    }, 
    desc: {
        type: String, 
        default: ""
    }, 
    rent: {
        type: Number, 
        default: 0
    }, 
    category: {
        type: String, 
        default: ""
    }, 
    garage: {
        type: Boolean, 
        default: false
    }
})

</script>

<template>
    <div class="single_property bg-secondary text-light rounded-3 my-2 p-4" style="min-height: 200px">
        <h4 class="text-info">{{ title }}</h4>     
        <h6>{{ desc }}</h6>     
        <h5>Rent: <span class="text-info fw-bold">{{ rent }}</span></h5>
        <h6>*** {{ garage ? 'Parking available' : 'No parking' }} ***</h6>
    </div>
</template>

