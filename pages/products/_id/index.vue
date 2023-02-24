<template>
  <div>
    <div>
      <div class="grid grid-cols-2 gap-5">
        <section class="mx-auto mt-20">
          <img :src="dataIphone.imageDefault" alt="" class="w-96" />
        </section>
        <section class="mt-20 align-middle">
          <div class="mb-5">
            <h1 class="text-2xl">{{ dataIphone.name }}</h1>
            <p class="text-red-600 text-lg">Rp. {{ dataIphone.price }}</p>
          </div>

          <div class="mb-5">
            <h3 class="text-lg pb-1">Color</h3>
            <div class="flex gap-5">
              <div class="flex gap-3">
                <label
                  class="cursor-pointer"
                  v-for="color in dataIphone.colors"
                >
                  <input
                    class="peer sr-only"
                    type="radio"
                    name="color"
                    @click="changeColor(`${color.name}`)"
                  />
                  <div
                    :style="`background-color: ${color.hexCode}`"
                    class="peer-checked:outline peer-checked:outline-black px-3 py-3 rounded-full"
                  ></div>
                </label>
              </div>
            </div>
          </div>

          <div class="mb-5">
            <h3 class="text-lg pb-1">Pilihan Kartu Sim</h3>
            <div class="flex gap-3">
              <label class="cursor-pointer">
                <input class="peer sr-only" type="radio" name="simcard" />
                <div
                  class="text-slate-500 outline outline-slate-200 peer-checked:text-white peer-checked:bg-[#0CDE77] px-5 py-1 rounded"
                >
                  Tanpa Kartu Sim
                </div>
              </label>
              <label class="cursor-pointer">
                <input class="peer sr-only" type="radio" name="simcard" />
                <div
                  class="text-slate-500 outline outline-slate-200 peer-checked:text-white peer-checked:bg-[#0CDE77] px-5 py-1 rounded"
                >
                  Telkomsel
                </div>
              </label>
            </div>
          </div>
          <div class="mb-5">
            <div>
              <h3 class="text-lg pb-1">
                Stok : {{ dataIphone.stok }}
              </h3>
            </div>
          </div>
          <div class="flex gap-3">
            <button
              class="bg-[#0CDE77] text-white text-lg py-1 px-12 rounded hover:bg-transparent hover:text-[#0CDE77] hover:outline"
            >
              Buy Now
            </button>
            <button
              class="bg-[#0CDE77] text-white text-lg py-1 px-12 rounded hover:bg-transparent hover:text-[#0CDE77] hover:outline"
            >
              Add To Cart
            </button>
          </div>
        </section>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      dataIphone: {
        ...this.$route.params.id,
      },
      // dataIphone : {
      //     image: this.$route.params.id.colors[0].image,
      //     quantity: this.$route.params.id.colors[0].stock,
      //      ...this.$route.params.id
      // },
    };
  },
  methods: {
    changeColor(value) {
      // for (const color in this.dataIphone.colors) {
      // }
      if (value === "Grey") {
        this.dataIphone.imageDefault = "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/eb9131cee70da1c0a2e42acb2d53c127/helix/01-APPLE-8DVPHAPPA-APPMQC23ID-A-Space%20Black1.jpg"
        this.dataIphone.stok = this.dataIphone.colors[0].stock
      }
      else if (value === "Silver") {
        this.dataIphone.imageDefault = "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/0fd984c34049b3b308520a4388c931b6/helix/01-APPLE-8DVPHAPPA-APPMQC33ID-A-Silver1.jpg";
        this.dataIphone.stok = this.dataIphone.colors[1].stock
      }
      else if (value === "Gold") {
        this.dataIphone.imageDefault = "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/aa8850cf144f6d1a64f733944ad46b55/helix/01-APPLE-8DVPHAPPA-APPMQC43ID-A-Gold1.jpg";
        this.dataIphone.stok = this.dataIphone.colors[2].stock
      }
      else {
        this.dataIphone.imageDefault = "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/25976fbb8f069a6e2e05c1ae7c1380eb/helix/01-APPLE-8DVPHAPPA-APPMQC53ID-A-Deep%20Purple1.jpg"
        this.dataIphone.stok = this.dataIphone.colors[3].stock
      }
      // console.log(color);
    },
  },
};
</script>
<style>
/*  :style="`background-color: ${color.name}`" */
</style>
