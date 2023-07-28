<template>
    <div class="h-[400px] bg-contain relative" :style="{ backgroundImage: 'url(./bluehouse_exterior_1920w.jpg)' }" >
        <div class="absolute h-[400px] inset-0 opacity-70 top-[0px]" style="background: linear-gradient(180deg, rgba(59, 77, 129, 0.7) 70%, rgba(59, 77, 129, 0));"></div>
        <div class="relative w-full h-full flex  justify-center items-center backdrop-brightness-[.4]">
            <div class="text-white w-2/3 text-center">
                <h3 class="text-4xl ">Find Your Dream Home</h3>
                <p class="mt-2">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis ultricies placerat felis. Praesent consectetur vestibulum nibh, vitae vulputate odio.</p>
                <div class="flex items-center justify-center gap-x-4 mt-5">
                    <button :class="activeTab == 1 ? 'btn-active':'btn-normal'" @click="activeTab = 1">Rent</button>
                    <button :class="activeTab == 2 ? 'btn-active':'btn-normal'" @click="activeTab = 2">Sale</button>
                </div>

                <div class="mt-5 bg-white rounded-md py-4 px-6 grid grid-cols-4 gap-x-5">
                    <div class="block text-left">
                        <label class="text-gray-700 text-sm">Locations</label>
                        <el-select fit-input-width v-model="formData.location" placeholder="Select" size="large" class="no-border">
                            <el-option
                                v-for="item in locations"
                                :key="item.value"
                                :label="item.label"
                                :value="item.value"
                            />
                        </el-select>
                    </div>
                    <div class="block text-left">
                        <label class="text-gray-700 text-sm">Locations</label>
                        <el-select fit-input-width class="no-border" v-model="formData.location" placeholder="Select" size="large">
                            <el-option
                                v-for="item in locations"
                                :key="item.value"
                                :label="item.label"
                                :value="item.value"
                            />
                        </el-select>
                    </div>
                    <div class="block text-left">
                        <label class="text-gray-700 text-sm">Locations</label>
                        <el-select fit-input-width class="no-border" v-model="formData.location" placeholder="Select" size="large">
                            <el-option
                                v-for="item in locations"
                                :key="item.value"
                                :label="item.label"
                                :value="item.value"
                            />
                        </el-select>
                    </div>
                    <div class="flex justify-end">
                        <button class="bg-indigo-500 px-4 py-[1px] rounded-md mt-4 h-[40px]">Search</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
    import { reactive,ref } from "vue";

    const formData = reactive({
        location:''
    });

    const locations = reactive([]);

    const activeTab = ref(1);
</script>
<style scoped>
    .btn-active{
        @apply bg-indigo-500 px-4 py-[6px] rounded-sm;
    }
    .btn-normal{
        @apply bg-white text-indigo-500 px-4 py-[6px] rounded-sm;
    }
</style>