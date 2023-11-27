<script setup>
import {reactive} from 'vue'

const products = reactive( [
    {
        image: "/src/assets/pc.jpg",
        number: "01",
        id:1,
        title: "reviving Retro PCs",
        description: "What happens when old PCs are given modern upgrades?"
    },
    {   
        image: '/src/assets/laptop.jpg',
        number: "02",
        id:2,
        title: "Top 10 Laptops of 2022",
        description: " Our best picks for various needs and budgets."
    },
    {   
        image: '/src/assets/gaming.jpg',
        number: "03",
        id:3,
        title: "The Growth of Gaming ",
        description: "How the pandemic has sparked fresh opportunities."
    }
    
 
])
</script>

<template>

    <section class="flex flex-col gap-5 mt-10 md:flex-row ">
        <div v-for="product in products" :key="product.id" >
            <div class=" flex flex-row p-4 gap-5">

                <div class="">
                    <img :src="product.image">
                </div>
                <div class="flex flex-col ">  
                    <p class="text-[#a0a0a0]  text-3xl">{{ product.number }}</p> 
                    <a href="" class=" hover:text-[#E8AD4F] font-bold ">{{ product.title }}</a>
                    <p class="text-[#131313] text-sm">{{ product.description }}</p>
                </div>
            </div>
        </div>
    </section>
</template>