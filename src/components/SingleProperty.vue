<template>
    <div class="h-full">
        <el-image fit="fill" lazy alt="gallery" class="block h-full w-full rounded-lg object-cover object-center" :src="src" />
    </div>
</template>
<script setup>
    const props = defineProps({
        src: String
    });
</script>