<script setup>
import {reactive} from 'vue'
let menu = reactive({isOpen: false});
function openMenu(){
menu.isOpen = !menu.isOpen;
 
}
</script>

<template>

        <nav class="relative pb-10" >
           <div class="transition-opacity md:hidden">

               <img src="../assets/icon-menu.svg" class="absolute right-4 top-2 z-10 " @click="openMenu">
               
               <div  class="relative bg-white" v-if="menu.isOpen">
                <div class="  flex flex-col gap-2 font-extrabold h-screen items-center pt-20 ">
                    <a href="#" class="hover:opacity-80  hover:underline">Home</a>
                    <a href="#" class="hover:opacity-80  hover:underline">New</a>
                    <a href="#" class="hover:opacity-80  hover:underline">Popular</a>
                    <a href="#" class="hover:opacity-80  hover:underline">Trending</a>
                    <a href="#" class="hover:opacity-80  hover:underline">Categories</a>
               
                </div>
            </div>
            </div>
            <div class="hidden md:flex justify-between p-2 ">
                
                <div class="w-[40px]">
                    <img src="../assets/logo.svg" alt="" class="opacity-90 cursor-pointer">
                </div>
                
                <div class="flex gap-4 mr-2 opacity-80">
                    <a href="#" class="hover:opacity-80  hover:underline">Home</a>
                    <a href="#" class="hover:opacity-80  hover:underline">New</a>
                    <a href="#" class="hover:opacity-80  hover:underline">Popular</a>
                    <a href="#" class="hover:opacity-80  hover:underline">Trending</a>
                    <a href="#" class="hover:opacity-80  hover:underline">Categories</a>
                    
                    
                </div>
            </div>
            </nav>
</template>