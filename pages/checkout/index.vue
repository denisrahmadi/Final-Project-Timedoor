<template>
    <div>
        <h1 class="text-center text-2xl font-bold my-16">Checkout</h1>
        <section class="container ml-20 mt-10 grid grid-cols-2">
            <div class="block">
                <div class="flex gap-10 max-w-xl border-b-2 border-slate-400 rounded">
    
                    <div>
                        <img
                            class="w-40" 
                            src="https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/eb9131cee70da1c0a2e42acb2d53c127/helix/01-APPLE-8DVPHAPPA-APPMQC23ID-A-Space%20Black1.jpg"
                            alt=""
                        >
                    </div>
                    <div class="pt-14 text-sm font-[roboto, serif]">
                        <p class="w-44">iPhone 14 Pro Max 128 GB</p>
                        <p>Grey</p>
                    </div>
                    <div class="pt-14 ml-16">
                        <div class="flex">
                            <button @click="minQuantity" class="hover:text-red-400"><i class="fa-solid fa-minus"></i></button>
                            <p class="inline mx-3 outline outline-1 outline-slate-400 px-3 rounded">{{ quantity }}</p>
                            <button @click="plusQuantity" class="hover:text-green-400"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                    <div class="pt-14 hover:text-red-600">
                        <button><i class="fa-solid fa-trash-can"></i></button>
                    </div>
                </div>
            </div>
            <div>
                <div class="bg-slate-300 w-96 p-5 rounded">
                    <table>
                        <tr>
                            <td>iPhone 14 Pro Max 128 GB</td>
                            <td class="pl-8">Rp. 20999000</td>
                        </tr>
                        <tr>
                            <td>iPhone 14 Pro Max 128 GB</td>
                            <td class="pl-8">Rp. 20999000</td>
                        </tr>
                        <tr>
                            <td>iPhone 14 Pro Max 128 GB</td>
                            <td class="pl-8">Rp. 20999000</td>
                        </tr>
                        <tr>
                            <td>iPhone 14 Pro Max 128 GB</td>
                            <td class="pl-8">Rp. 20999000</td>
                        </tr>
                        <tr>
                            <td class="pt-8 font-bold">Total</td>
                            <td class="pl-8 pt-8 font-bold">Rp. 90999000</td>
                        </tr>
                    </table>
                </div>
            </div>
        </section>
    </div>
</template>
<script>
export default {
    data() {
        return {
            quantity: 0
        }
    },
    methods: {
        plusQuantity(){
            this.quantity++
        },
        minQuantity(){
            this.quantity--
            if (this.quantity < 0) {
                this.quantity = 0
            }
        }
    },
}
</script>
<style>
    
</style>