<template>
    <div class=" bg-white pb-10">
        <div class="container mx-auto px-5 py-2 lg:px-32 lg:pt-12">
            <div class="text-gray-900 text-center mb-5">
                <h3 class="text-2xl font-semibold">Properties By Area</h3>
                <p class="mt-2 text-gray-500">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis ultricies placerat felis. Praesent consectetur vestibulum nibh, vitae vulputate odio.</p>
            </div>
            <div class="grid grid-cols-4 gap-x-5 mt-3">
                <div v-for="(property,key) in properties" :key="key" class="border p-2 rounded-lg">
                    <PropertyDetails :property="property"/>
                </div>
            </div>

            <div class="flex justify-center mx-auto mt-7">
                <button class="bg-[#4A60A1] px-4 py-2 text-white rounded-[3px]">Load More Listing</button>
            </div>
        </div>
    </div>
</template>
<script setup>
    
    const properties = [
        {
            title:'92 ALLIUM PLACE, ORLANDO FL 32827',
            price:256889,
            car:2,
            bathtub:4,
            sqft:2564
        },
        {
            title:'92 ALLIUM PLACE, ORLANDO FL 32827',
            price:256889,
            car:2,
            bathtub:4,
            sqft:2564
        },
        {
            title:'92 ALLIUM PLACE, ORLANDO FL 32827',
            price:256889,
            car:2,
            bathtub:4,
            sqft:2564
        },
        {
            title:'92 ALLIUM PLACE, ORLANDO FL 32827',
            price:256889,
            car:2,
            bathtub:4,
            sqft:2564
        },
    ];
</script>