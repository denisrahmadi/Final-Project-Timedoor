<template>
    <div>
        <div class="mt-32">
            <ul class="flex justify-center gap-16">
                <li v-for="(item, index) in guaranteeData" :key="index" >
                    <div class="overflow-hidden w-40 text-left">
                        <img :src="item.logo" alt="" class="w-[125px]">
                        <h5 class="font-bold mt-4">{{ item.title }}</h5>
                        <p class="font-normal">{{ item.detail }}</p>
                    </div>
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
                    title: "GARANSI iGapple",
                    detail: "Produk bergaransi resmi",
                },
                {
                    logo: "https://cdn-icons-png.flaticon.com/512/1621/1621563.png",
                    title: "iGapple MEMBERSHIP",
                    detail: "Dapatkan penawaran menarik khusus member",
                },
                {
                    logo: "https://cdn-icons-png.flaticon.com/128/4021/4021708.png",
                    title: "0% CICILAN",
                    detail: "Makin terjangkau dengan cicilan tanpa bunga",
                },
                {
                    logo: "https://cdn-icons-png.flaticon.com/128/709/709790.png",
                    title: "PENGIRIMAN CEPAT & AMAN",
                    detail: "Jaminan barang rusak",
                },
            ]
        }
    },
}
</script>
<style>
    
</style>