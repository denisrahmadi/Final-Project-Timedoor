<template>
    <div>
        <div class="container mt-20">
            <h3 class="text-center font-semibold mb-14 text-xl">Our Benefits</h3>
            <ul class="grid justify-center gap-3 grid-cols-4">
                <li v-for="(item, index) in guaranteeData" :key="index" class="w-40 mx-auto">
                        <img :src="item.logo" alt="" class="w-[100px]">
                    <h5 class="font-bold mt-1">{{ item.title }}</h5>
                    <p class="text-lef">{{ item.detail }}</p>
                </li>
            </ul>
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            guaranteeData: [
                {
                    logo: "https://cdn-icons-png.flaticon.com/512/3734/3734879.png",
                    title: "GARANSI",
                    detail: "Produk bergaransi resmi",
                },
                {
                    logo: "https://cdn-icons-png.flaticon.com/512/1621/1621563.png",
                    title: "MEMBERSHIP",
                    detail: "Dapatkan penawaran menarik khusus member",
                },
                {
                    logo: "https://cdn-icons-png.flaticon.com/128/4021/4021708.png",
                    title: "0% CICILAN",
                    detail: "Makin terjangkau dengan cicilan tanpa bunga",
                },
                {
                    logo: "https://cdn-icons-png.flaticon.com/128/709/709790.png",
                    title: "FREE DELIVERY",
                    detail: "Jaminan barang rusak",
                },
            ]
        }
    },
}
</script>
<style>
    
</style>