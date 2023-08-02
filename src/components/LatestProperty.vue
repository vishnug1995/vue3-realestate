<template>
    <div class=" bg-white pb-10">
        <div class="container mx-auto px-5 py-2 lg:px-32 lg:pt-12">
            <div class="text-gray-900 text-center mb-5">
                <h3 class="text-2xl font-semibold">Properties By Area</h3>
                <p class="mt-2 text-gray-500">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis ultricies placerat felis. Praesent consectetur vestibulum nibh, vitae vulputate odio.</p>
            </div>
            <div class="grid grid-cols-4 gap-x-5 mt-3">
                <div v-for="(property,key) in properties" :key="key" class="border p-2 rounded-lg">
                    <el-image src="/1.jpg" class="rounded-lg"/>
                    <h3>{{ property.title }}</h3>

                    <p class="text-[#4A60A1] mt-6 text-[15px]">${{ property.price }}</p>

                    <div class="mt-5 flex items-center gap-x-5 text-[#6D737A]">
                        <div class="flex items-center">
                            <BxCar class="text-[17px] "/>
                            <span class="block mt-[0.1rem] ml-1">{{ property.car }}</span>
                        </div>
                        <div class="flex items-center">
                            <BxBath class="text-[17px]"/>
                            <span class="block mt-[0.1rem] ml-1">{{ property.bathtub }}</span>
                        </div>
                        <div class="flex items-center">
                            <BxBuildingHouse class="text-[17px]"/>
                            <span class="block mt-[0.1rem] ml-1">{{ property.sqft }} sqft</span>
                        </div>
                    </div>

                    <div class="flex items-center mt-5 justify-between">
                        <div class="flex items-center">
                            <img src="https://i.pravatar.cc/30" class="rounded-full h-[30px] w-auto shadow-md"/>
                            <span class="ml-2">Wilfred</span>
                        </div>

                        <div class="flex items-center gap-x-3">
                            <div class="bg-[#EDEFF6] p-[3px]"><AnOutlinedShareAlt/></div>
                            <div class="bg-[#EDEFF6] p-[3px]"><AkHeart/></div>
                            <div class="bg-[#EDEFF6] p-[3px]"><AnOutlinedPlus/></div>
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
    import { BxCar,BxBath,BxBuildingHouse,AnOutlinedShareAlt,AkHeart,AnOutlinedPlus } from "@kalimahapps/vue-icons";
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