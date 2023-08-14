<template>
    <div class=" bg-white p-12">
        <div class="grid grid-cols-4 gap-4">
            <div class="col-span-1 space-y-2">
                <div class="flex flex-shrink-0 items-center">
                    <img class="h-10 w-auto" src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=500" alt="Your Company">
                    <div class="block ml-2">
                        <div class="text-xl font-bold uppercase leading-none">Real</div>
                        <span class="text-sm font-bold leading-none">Estate</span>
                    </div>
                </div>

                <h4 class="text-[22px] text-black">Contact Us</h4>
                <p class="text-black/50">Call : +123 400 123</p>
                <p class="text-black/50">Integer a lectus lorem. Etiam dignissim <br/>
                suscipit orci eget molestie.</p>
                <p>Email : example@gmail.com</p>

                <div>
                    <ul class="flex items-center gap-x-3">
                        <li>
                            <div class="icon-wrapper"><BxFacebook class="icon"/></div>
                        </li>
                        <li>
                            <div class="icon-wrapper"><BxTwitter class="icon"/></div>
                        </li>
                        <li>
                            <div class="icon-wrapper"><BxYoutube class="icon"/></div>
                        </li>
                        <li>
                            <div class="icon-wrapper"><BxInstagram class="icon"/></div>
                        </li>
                        <li>
                            <div class="icon-wrapper"><BxLinkedin class="icon"/></div>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="col-span-1">
                <h4 class="text-[22px] text-black">Features</h4>

                <ul class="grid grid-cols-1 gap-y-4 mt-5">
                    <li>Home</li>
                    <li>Become a host</li>
                    <li>Pricing</li>
                    <li>Blog</li>
                    <li>Contact</li>
                </ul>
            </div>
            <div class="col-span-1">
                <h4 class="text-[22px] text-black">Company</h4>

                <ul class="grid grid-cols-1 gap-y-4 mt-5">
                    <li><router-link to="about">About Us</router-link></li>
                    <li>Press</li>
                    <li>Contact</li>
                    <li>Career</li>
                    <li>Blog</li>
                </ul>
            </div>

            <div class="col-span-1">
                <h4 class="text-[22px] text-black">Terms and policies</h4>

                <ul class="grid grid-cols-1 gap-y-4 mt-5">
                    <li>Terms of servies</li>
                    <li>Privacy policy</li>
                    <li>Security</li>
                </ul>
            </div>
        </div>
    </div>
</template>
<script setup>
    import { BxFacebook,BxTwitter,BxYoutube,BxInstagram,BxLinkedin } from "@kalimahapps/vue-icons";
</script>
<style scoped lang="scss">
    .icon-wrapper{
        @apply bg-[#EDEFF6] p-[12px];
        .icon{
            @apply text-[#4A60A1] text-[20px];
        }
    }
</style>