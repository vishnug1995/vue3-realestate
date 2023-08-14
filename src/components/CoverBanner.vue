<template>
    <div class="cover" style="background-image: url('cover.avif');">
        <div class="z-10 absolute inset-0 opacity-70" style="background: linear-gradient(rgba(6, 48, 83, 0.9) 100%, rgb(9 73 255 / 0%));"></div>
        <div class="relative z-20 h-full">
            <div class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2">  
                <h4 class="text-white text-[52px]">Properties</h4>
                <el-breadcrumb separator="/" class="flex justify-center ">
                    <el-breadcrumb-item :to="{ path: '/' }" class="text-white">Home</el-breadcrumb-item>
                    <el-breadcrumb-item>Properties</el-breadcrumb-item>
                </el-breadcrumb>
            </div> 
        </div> 
    </div>
</template>
<style>
.cover{
    height: 240px;
    background-position: 0 -620px;
    background-repeat: no-repeat;
    width: 100%;
    background-size: cover;
    @apply relative
}

</style>