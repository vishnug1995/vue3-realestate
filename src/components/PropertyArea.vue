<template>
<div class="container mx-auto px-5 py-2 lg:px-32 lg:pt-12">
    <div class="text-gray-900 text-center mb-5">
        <h3 class="text-2xl font-semibold">Properties By Area</h3>
        <p class="mt-2 text-gray-500">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis ultricies placerat felis. Praesent consectetur vestibulum nibh, vitae vulputate odio.</p>
    </div>
    <div class="-m-1 flex flex-wrap md:-m-2">
        <div v-for="(gallery,key) in galleries" :class="gallery.class" :key="key">
            <div v-for="(sg,key_1) in gallery.children"  :class="sg.class" :key="key_1">
                <SingleProperty :src="sg.src"/>
            </div>
        </div>
    </div>
</div>
</template>
<script setup>
    const galleries = [
      {
        id: 1,
        class: "flex w-1/2 flex-wrap",
        children: [
            {
                id: 1,
                class: "w-1/2 p-1 md:p-2",
                src: "/1.jpg"
            },
            {
                id: 2,
                class: "w-1/2 p-1 md:p-2",
                src: "/2.jpg"
            },
            {
                id: 3,
                class: "w-full p-1 md:p-2",
                src: "/3.jpg"
            }
        ]
      },
      {
        id: 2,
        class: "flex w-1/2 flex-wrap",
        children: [
            {
                id: 4,
                class: "w-full p-1 md:p-2",
                src: "/4.jpg"
            },
            {
                id: 5,
                class: "w-1/2 p-1 md:p-2",
                src: "/5.jpg"
            },
            {
                id: 6,
                class: "w-1/2 p-1 md:p-2",
                src: "/6.jpg"
            }
        ]
      }
    ];

</script>
