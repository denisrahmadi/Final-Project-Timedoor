<template>
    <div>
        <ul  class="grid gap-4 mt-4 sm:grid-cols-2 lg:grid-cols-4">
            <li 
                v-for="(product, index) in productHomePage"
                :key="index"
            >
                <nuxt-link to="#" class="mx-auto group">
                    <img
                        :src="product.image"
                        alt=""
                        class="h-[350px] w-full object-cover transition duration-500 group-hover:scale-105 sm:h-[450px]"
                    />
                    <div class="relative ml-auto mr-auto pt-3 bg-white">
                        <h3 class="flex justify-center text-lg text-gray-700 group-hover:underline group-hover:underline-offset-8">
                        {{ product.name }}
                        </h3>
                        <p class="flex justify-center mt-2">
                        <span class="tracking-wider text-red-500"> Rp. {{ product.price }} </span>
                        </p>
                    </div>
                </nuxt-link>
            </li>

        </ul>
    </div>
</template>
<script>
export default {
    
}
</script>
<style>
    
</style>