<script setup>
import AsideNews from './AsideNews.vue';


</script>

<template>
            <section class=" md:flex  justify-around gap-4 ">
                

                    <div class="flex flex-col ">
                        <img src="../assets/image-web-3-desktop.jpg" >
                        <div class=" sm:flex flex-col md:flex md:flex-row justify-between justify-between">

                            <div class=" flex flex-col   p-2 text-2xl font-bold  w-[300px]">
                                <h2 class="">The Bright </h2>
                                <p > Future of</p>
                                <p>Web 3.0?</p>
                                
                            </div>
                            
                            <div class=" flex flex-col gap-2 w-[380px] p-4">
                                <h3 class="opacity-90 ">We dive into the next evolution of the web that claims to put the power of the platforms back into the hands of the people. But is it really fulfilling its promise? </h3>
                                <button 
                                class="bg-[#F35D4F] p-1 w-fit text-[#fff] 
                                 uppercase  pr-2 pl-2 font-serif 
                                 hover:text-opacity-80 hover:text-[#000]
                                 "
                                 >red more</button>
                            </div>
                        </div>
                        
                    </div>
                     
                
                <AsideNews />
            </section>
</template>