<template>
    <div class=" bg-[#EDEFF6] pb-10">
        <div class="container mx-auto px-5 py-2 lg:px-32 lg:pt-12">
            <div class="text-gray-900 text-center mb-5">
                <h3 class="text-2xl font-semibold">Properties By Area</h3>
                <p class="mt-2 text-gray-500">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis ultricies placerat felis. Praesent consectetur vestibulum nibh, vitae vulputate odio.</p>
            </div>
            <div class="grid grid-cols-4 gap-x-16 mt-3">
                <div v-for="(property,key) in properties" :key="key" class="bg-white p-8">
                    <IcHomeAlt v-if="property.icon == 'IcHomeAlt'" class="text-[50px] text-blue-500"/>
                    <IcHomeShield v-if="property.icon == 'IcHomeShield'" class="text-[50px] text-blue-500"/>
                    <IcHomeTemperatureIn v-if="property.icon == 'IcHomeTemperatureIn'" class="text-[50px] text-blue-500"/>
                    <IcHomeSale v-if="property.icon == 'IcHomeSale'" class="text-[50px] text-blue-500"/>

                    <h3 class="mt-3 text-[20px] font-bold">{{ property.title }}</h3>
                    <p class="mt-2">{{ property.description }}</p>

                    <button class="text-blue-500 mt-3">Read More</button>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
    import { IcHomeAlt,IcHomeShield,IcHomeTemperatureIn,IcHomeSale } from "@kalimahapps/vue-icons";
    const properties = [{
        icon:'IcHomeAlt',
        title:'Sell Your Home',
        description:'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis venenatis dolor, eget efficitur lectus.'
    },
    {
        icon:'IcHomeShield',
        title:'Rent Your Home',
        description:'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis venenatis dolor, eget efficitur lectus.'
    },
    {
        icon:'IcHomeTemperatureIn',
        title:'Buy a home',
        description:'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis venenatis dolor, eget efficitur lectus.'
    },
    {
        icon:'IcHomeSale',
        title:'Free Marketing',
        description:'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis venenatis dolor, eget efficitur lectus.'
    }];
</script>