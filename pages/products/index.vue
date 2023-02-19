<template>
  <div>
    <Navbar />
    <div class="m-20">
        <h1 class="font-bold text-xl">iPhone</h1>
        <ul  class="grid gap-4 mt-4 sm:grid-cols-2 lg:grid-cols-4">
                <li 
                  v-for="(product, index) in dataIphones"
                  :key="index"
                >
                  <nuxt-link to="#" class="mx-auto group">
                    <img
                      :src="product.image[1]"
                      alt=""
                      class="h-[250px] w-full object-cover transition duration-500 group-hover:scale-105 sm:h-[350px]"
                    />
      
                    <div class="relative ml-auto mr-auto pt-3 bg-white">
                      <h3 class="flex justify-center text-lg text-gray-700 group-hover:underline group-hover:underline-offset-4 group-hover:decoration-[#0CDE77] delay-100">
                        {{ product.name }}
                      </h3>
                      <p class="flex justify-center mt-2">
                        <span class="tracking-wider text-red-500"> Rp. {{ product.price[1] }} </span>
                      </p>
                    </div>
                  </nuxt-link>
                </li>
      
        </ul>
    </div>
    <div class="m-20">
        <h1 class="font-bold text-xl">MacBook</h1>
        <ul  class="grid gap-4 mt-4 sm:grid-cols-2 lg:grid-cols-4">
                <li 
                  v-for="(product, index) in dataMacbooks"
                  :key="index"
                >
                  <nuxt-link to="#" class="mx-auto group">
                    <img
                      :src="product.image[1]"
                      alt=""
                      class="h-[250px] w-full object-cover transition duration-500 group-hover:scale-105 sm:h-[350px]"
                    />
      
                    <div class="relative ml-auto mr-auto pt-3 bg-white">
                      <h3 class="flex justify-center text-lg text-gray-700 group-hover:underline group-hover:underline-offset-4 group-hover:decoration-[#0CDE77]" >
                        {{ product.name }}
                      </h3>
                      <p class="flex justify-center mt-2">
                        <span class="tracking-wider text-red-500"> Rp. {{ product.price[1] }} </span>
                      </p>
                    </div>
                  </nuxt-link>
                </li>
      
        </ul>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
        dataIphones: [
            {
                name: "iPhone 14 Pro Max",
                price: ["20.999.000", "23.999.000", "27.999.000", "31.999.000"],
                capacity: [128, 256, 512, 1],
                image: [
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/eb9131cee70da1c0a2e42acb2d53c127/helix/01-APPLE-8DVPHAPPA-APPMQC23ID-A-Space%20Black1.jpg",
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/0fd984c34049b3b308520a4388c931b6/helix/01-APPLE-8DVPHAPPA-APPMQC33ID-A-Silver1.jpg",
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/aa8850cf144f6d1a64f733944ad46b55/helix/01-APPLE-8DVPHAPPA-APPMQC43ID-A-Gold1.jpg",
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/25976fbb8f069a6e2e05c1ae7c1380eb/helix/01-APPLE-8DVPHAPPA-APPMQC53ID-A-Deep%20Purple1.jpg",
                ],
                color: ["Grey", "Silver", "Gold", "Purple"],
            },
            {
                name: "iPhone 13 Pro Max",
                price: ["19.499.000", "21.499.000", "25.499.000", "28.999.000"],
                capacity: [128, 256, 512, 1],
                image: [
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/fe2e7f42304e7811d3380ac7bef3e37b/helix/01-APPLE-8DVPHAPP0-APPMND23ID-A-AlpineGreenRevSS.jpg",
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/7175e59258ed514d30b69baa62327a31/helix/01-APPLE-8DVPHAPP0-APPMLLN3ID-A-SierraBlueRevSS.jpg",
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/fc061105a4505afba461ab571639b3c8/helix/01-APPLE-8DVPHAPP0-APPMLLM3ID-A-GoldRevSS.jpg",
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/483789a556311c40f40625045801bf8f/helix/01-APPLE-8DVPHAPP0-APPMLLL3ID-A-SilverRevSS.jpg",
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/e9b0262357f4ee68b0d837a2d3857015/helix/01-APPLE-8DVPHAPP0-APPMLLK3ID-A-GraphiteRevSS.jpg",
                ],
                color: ["Green", "Blue", "Gold", "Silver", "Grey"],
            },
            {
                name: "iPhone 14 Pro Max",
                price: ["20.999.000", "23.999.000", "27.999.000", "31.999.000"],
                capacity: [128, 256, 512, 1],
                image: [
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/eb9131cee70da1c0a2e42acb2d53c127/helix/01-APPLE-8DVPHAPPA-APPMQC23ID-A-Space%20Black1.jpg",
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/0fd984c34049b3b308520a4388c931b6/helix/01-APPLE-8DVPHAPPA-APPMQC33ID-A-Silver1.jpg",
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/aa8850cf144f6d1a64f733944ad46b55/helix/01-APPLE-8DVPHAPPA-APPMQC43ID-A-Gold1.jpg",
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/25976fbb8f069a6e2e05c1ae7c1380eb/helix/01-APPLE-8DVPHAPPA-APPMQC53ID-A-Deep%20Purple1.jpg",
                ],
                color: ["Grey", "Silver", "Gold", "Purple"],
            },
            {
                name: "iPhone 13 Pro Max",
                price: ["19.499.000", "21.499.000", "25.499.000", "28.999.000"],
                capacity: [128, 256, 512, 1],
                image: [
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/fe2e7f42304e7811d3380ac7bef3e37b/helix/01-APPLE-8DVPHAPP0-APPMND23ID-A-AlpineGreenRevSS.jpg",
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/7175e59258ed514d30b69baa62327a31/helix/01-APPLE-8DVPHAPP0-APPMLLN3ID-A-SierraBlueRevSS.jpg",
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/fc061105a4505afba461ab571639b3c8/helix/01-APPLE-8DVPHAPP0-APPMLLM3ID-A-GoldRevSS.jpg",
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/483789a556311c40f40625045801bf8f/helix/01-APPLE-8DVPHAPP0-APPMLLL3ID-A-SilverRevSS.jpg",
                    "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/e9b0262357f4ee68b0d837a2d3857015/helix/01-APPLE-8DVPHAPP0-APPMLLK3ID-A-GraphiteRevSS.jpg",
                ],
                color: ["Green", "Blue", "Gold", "Silver", "Grey"],
            },
        ],
        dataMacbooks: [
            {
                name: "MacBook Pro M2 13.3 inch",
                price: ["20.999.000", "24.999.000"],
                capacity: [256, 512],
                image: [
                        "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/39fd68ba71526a38d272161698789e95/helix/01-APPLE-8DVLPAPP0-APPMNEQ3ID-A-SilverRevSS.jpg",
                        "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/84d62c4bf14ffc55749cc0254d754a91/helix/01-APPLE-8DVLPAPP0-APPMNEJ3ID-A-SpaceGrayRevSS.jpg"	
                    ],
                color: ["Silver", "Grey"]
            },
            {
                name: "MacBook Air 13.6 inch M2",
                price: ["19.999.000", "24.999.000"],
                capacity: [256, 512],
                image: [
                        "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/06b9ae76b44fb7228c37816230d215bd/helix/01-APPLE-8DVLPAPP0-APPMLXX3ID-A-Space%20Grey.jpg",
                        "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/85ebf4573e3b82010f2e0b4d6277f72f/helix/01-APPLE-8DVLPAPP0-APPMLY03ID-A-Silver.jpg",
                        "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/bba721ad2010c0c2de566886dad995a7/helix/01-APPLE-8DVLPAPP0-APPMLY23ID-A-Starlight.jpg",
                        "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/f6e4b695f544e8e1919d1320ae3cfa9d/helix/01-APPLE-8DVLPAPP0-APPMLY43ID-A-Midnight.jpg"		
                    ],
                color: ["Grey", "Silver", "Starlight", "Midnight"]
            },
            {
                name: "MacBook Pro M2 13.3 inch",
                price: ["20.999.000", "24.999.000"],
                capacity: [256, 512],
                image: [
                        "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/39fd68ba71526a38d272161698789e95/helix/01-APPLE-8DVLPAPP0-APPMNEQ3ID-A-SilverRevSS.jpg",
                        "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/84d62c4bf14ffc55749cc0254d754a91/helix/01-APPLE-8DVLPAPP0-APPMNEJ3ID-A-SpaceGrayRevSS.jpg"	
                    ],
                color: ["Silver", "Grey"]
            },
            {
                name: "MacBook Air 13.6 inch M2",
                price: ["19.999.000", "24.999.000"],
                capacity: [256, 512],
                image: [
                        "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/06b9ae76b44fb7228c37816230d215bd/helix/01-APPLE-8DVLPAPP0-APPMLXX3ID-A-Space%20Grey.jpg",
                        "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/85ebf4573e3b82010f2e0b4d6277f72f/helix/01-APPLE-8DVLPAPP0-APPMLY03ID-A-Silver.jpg",
                        "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/bba721ad2010c0c2de566886dad995a7/helix/01-APPLE-8DVLPAPP0-APPMLY23ID-A-Starlight.jpg",
                        "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/f6e4b695f544e8e1919d1320ae3cfa9d/helix/01-APPLE-8DVLPAPP0-APPMLY43ID-A-Midnight.jpg"		
                    ],
                color: ["Grey", "Silver", "Starlight", "Midnight"]
            },
        ]
    };
  },
};
</script>
<style></style>
