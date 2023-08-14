<template>
    <div class="container mx-auto">
        <div class="grid grid-cols-5 gap-x-5 mt-3">
            <div v-for="(property,key) in properties" :key="key" class="border p-2 rounded-lg">
                <PropertyDetails :property="property"/>
            </div>
        </div>
    </div>
</template>
<script setup>
    import properties from '@/assets/json/property.json'

</script>