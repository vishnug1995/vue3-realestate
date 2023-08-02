<template>
    <div class=" bg-white pb-10">
        <div class="container mx-auto px-5 py-2 lg:px-32 lg:pt-12">
            <div class="text-gray-900 text-center mb-5">
                <h3 class="text-2xl font-semibold">Latest Properties Of Rent</h3>
                <p class="mt-2 text-gray-500">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis ultricies placerat felis. Praesent consectetur vestibulum nibh, vitae vulputate odio.</p>
            </div>
            <div class="grid grid-cols-4 gap-x-5 mt-3">
                <div v-for="(property,key) in properties" :key="key" class="relative h-[426px]">
                    <div style="background: linear-gradient(180deg, rgba(59, 77, 129, 0) -12.86%, rgba(59, 77, 129, 0.5) 106.85%);" class="w-full h-full z-10 absolute rounded-md "></div>
                    <el-image :src="`/${key+1}.jpg`" class="rounded-md h-full shadow-lg" fit="cover"></el-image>
                    <div class="w-full justify-center flex items-center gap-x-5 text-[#fff] absolute bottom-0 z-10 mb-[15px]">
                        <div class="flex items-center">
                            <LaMapMarkerAltSolid class="text-[17px] "/>
                            <span class="block mt-[0.1rem] ml-1">{{ property.place }}</span>
                        </div>
                        <div class="flex items-center">
                            <BxBuildingHouse class="text-[17px]"/>
                            <span class="block mt-[0.1rem] ml-1">{{ property.sqft }} sqft</span>
                        </div>
                    </div>
                </div>
            </div>

            <div class="flex justify-center mx-auto mt-7">
                <button class="bg-[#4A60A1] px-4 py-2 text-white rounded-[3px]">Load More Listing</button>
            </div>
        </div>
    </div>
</template>
<script setup>
    import { LaMapMarkerAltSolid,BxBuildingHouse } from "@kalimahapps/vue-icons";
    const properties = [
        {
            place:'Washington',
            sqft:2564
        },
        {
            place:'Washington',
            sqft:2564
        },
        {
            place:'Washington',
            sqft:2564
        },
        {
            place:'Washington',
            sqft:2564
        },
    ];
</script>