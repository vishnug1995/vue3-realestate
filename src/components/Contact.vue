<template>
    <div class=" bg-[#EDEFF6] pb-10">
        <div class="max-w-2xl  mx-auto py-2 pt-20">
            <div class="text-gray-900 text-center mb-5">
                <h3 class="text-2xl font-semibold">Contact Us</h3>
                <p class="mt-3 text-gray-500">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis ultricies placerat felis. Praesent consectetur vestibulum nibh, vitae vulputate odio.</p>
            </div>
            <div class="mt-5 mx-auto">
                <el-card shadow="never">
                    <div>
                        <h2 class="font-bold text-[20px]">Enquiry Form</h2>
                        <p>Are you looking for details about a certain property? Ask us a question using the form below.</p>

                        <div class="grid grid-cols-2 gap-3 mt-5">
                            <div class="col-span-1">
                                <el-input placeholder="First Name" size="large"/>
                            </div>
                            <div class="col-span-1">
                                <el-input placeholder="Second Name" size="large"/>
                            </div>
                            <div class="col-span-2">
                                <el-input placeholder="Email id" size="large"/>
                            </div>
                            <div class="col-span-2">
                                <el-input type="textarea" placeholder="Comments or questions" size="large"/>
                            </div>
                        </div>
                        <button class="mx-auto flex justify-center mt-3 w-[150px] bg-[#4A60A1] px-4 py-2 text-white rounded-[4px]">Submit</button>
                    </div>
                </el-card>
            </div>
        </div>
    </div>
</template>
<script setup>
    
</script>