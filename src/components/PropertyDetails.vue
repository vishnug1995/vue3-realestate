<template>
    <div>
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
</template>
<script setup>
    import { BxCar,BxBath,BxBuildingHouse,AnOutlinedShareAlt,AkHeart,AnOutlinedPlus } from "@kalimahapps/vue-icons";
    const props = defineProps({
        property: Object
    });
    
</script>