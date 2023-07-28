<template>
    <div class="h-full shadow-lg relative cursor-pointer">
        <div class="absolute top-0 m-[15px] z-20 text-white ">
            <div class="text-lg font-bold">{{ title }}</div>
            <div class="text-md">{{ listings }} listings</div>
        </div>
        <div class="relative h-full w-full rounded-lg overflow-hidden z-10">
            <div class="z-10 absolute inset-0 opacity-70" style="background: linear-gradient(180deg, rgba(59, 77, 129, 0.7) 70%, rgba(59, 77, 129, 0));"></div>
            <el-image fit="fill" lazy alt="gallery" class="block h-full w-full rounded-lg object-cover object-center" :src="src" />
        </div>
    </div>
</template>
<script setup>
    const props = defineProps({
        src: String,
        title: String,
        listings: Number
    });
</script>
<style>
.bg-gradient-to-t {
    background-image: linear-gradient(to top, rgba(0, 0, 0, 0.7), transparent);
}
</style>