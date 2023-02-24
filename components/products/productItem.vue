<template>
  <div>
    <div class="m-20">
      <h1 class="font-bold text-xl">iPhone</h1>
      <ul class="grid gap-4 mt-4 sm:grid-cols-2 md:grid-cols-4 lg:grid-cols-4">
        <li v-for="(product, index) in dataIphones" :key="index">
          <nuxt-link
            tag="a"
            :to="{ name: 'products-id', params: { id: product } }"
            class="mx-auto group"
            
          >
            <img
              :src="product.imageDefault"
              alt=""
              class="h-[250px] w-full object-cover transition duration-500 group-hover:scale-105 sm:h-[350px]"
            />
            <div class="relative ml-auto mr-auto pt-3 bg-white">
              <h3
                class="flex justify-center text-lg text-gray-700 group-hover:underline group-hover:underline-offset-4 group-hover:decoration-[#0CDE77]"
              >
                {{ product.name }}
              </h3>
              <p class="flex justify-center mt-2">
                <span class="tracking-wider text-red-500">
                  Rp. {{ product.price }}
                </span>
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
          name: "iPhone 14 Pro Max 128 GB",
          id: 1,
          price: 20999000,
          stok: 100,
          imageDefault: "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/eb9131cee70da1c0a2e42acb2d53c127/helix/01-APPLE-8DVPHAPPA-APPMQC23ID-A-Space%20Black1.jpg",
          colors: [
            {
              id: 101,
              name: "Grey",
              hexCode: "#403E3D",
              image:
                "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/eb9131cee70da1c0a2e42acb2d53c127/helix/01-APPLE-8DVPHAPPA-APPMQC23ID-A-Space%20Black1.jpg",
              altText: "Grey",
              stock: 110,
            },
            {
              id: 102,
              name: "Silver",
              hexCode: "#E3E3E5",
              image:
                "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/0fd984c34049b3b308520a4388c931b6/helix/01-APPLE-8DVPHAPPA-APPMQC33ID-A-Silver1.jpg",
              altText: "Silver",
              stock: 120,
            },
            {
              id: 103,
              name: "Gold",
              hexCode: "#FAE7D0",
              image:
                "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/aa8850cf144f6d1a64f733944ad46b55/helix/01-APPLE-8DVPHAPPA-APPMQC43ID-A-Gold1.jpg",
              altText: "Gold",
              stock: 130,
            },
            {
              id: 104,
              name: "Purple",
              hexCode: "#817688",
              image:
                "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/25976fbb8f069a6e2e05c1ae7c1380eb/helix/01-APPLE-8DVPHAPPA-APPMQC53ID-A-Deep%20Purple1.jpg",
              altText: "Purple",
              stock: 140,
            },
          ],
        },
        {
          name: "iPhone 14 Pro Max 256 GB",
          price: 23999000,
          stok: 100,
          imageDefault: "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/0fd984c34049b3b308520a4388c931b6/helix/01-APPLE-8DVPHAPPA-APPMQC33ID-A-Silver1.jpg",
          id: 2,
          colors: [
            {
              id: 101,
              name: "Grey",
              hexCode: "#403E3D",
              image:
                "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/eb9131cee70da1c0a2e42acb2d53c127/helix/01-APPLE-8DVPHAPPA-APPMQC23ID-A-Space%20Black1.jpg",
              altText: "Grey",
              stock: 100,
            },
            {
              id: 102,
              name: "Silver",
              hexCode: "#E3E3E5",
              image:
                "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/0fd984c34049b3b308520a4388c931b6/helix/01-APPLE-8DVPHAPPA-APPMQC33ID-A-Silver1.jpg",
              altText: "Silver",
              stock: 100,
            },
            {
              id: 103,
              name: "Gold",
              hexCode: "#FAE7D0",
              image:
                "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/aa8850cf144f6d1a64f733944ad46b55/helix/01-APPLE-8DVPHAPPA-APPMQC43ID-A-Gold1.jpg",
              altText: "Gold",
              stock: 100,
            },
            {
              id: 104,
              name: "Purple",
              hexCode: "#817688",
              image:
                "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/25976fbb8f069a6e2e05c1ae7c1380eb/helix/01-APPLE-8DVPHAPPA-APPMQC53ID-A-Deep%20Purple1.jpg",
              altText: "Purple",
              stock: 100,
            },
          ],
        },
        {
          name: "iPhone 14 Pro Max 512 GB",
          price: 27999000,
          stok: 100,
          imageDefault: "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/aa8850cf144f6d1a64f733944ad46b55/helix/01-APPLE-8DVPHAPPA-APPMQC43ID-A-Gold1.jpg",
          id: 3,
          colors: [
            {
              id: 101,
              name: "Grey",
              hexCode: "#403E3D",
              image:
                "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/eb9131cee70da1c0a2e42acb2d53c127/helix/01-APPLE-8DVPHAPPA-APPMQC23ID-A-Space%20Black1.jpg",
              altText: "Grey",
              stock: 100,
            },
            {
              id: 102,
              name: "Silver",
              hexCode: "#E3E3E5",
              image:
                "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/0fd984c34049b3b308520a4388c931b6/helix/01-APPLE-8DVPHAPPA-APPMQC33ID-A-Silver1.jpg",
              altText: "Silver",
              stock: 100,
            },
            {
              id: 103,
              name: "Gold",
              hexCode: "#FAE7D0",
              image:
                "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/aa8850cf144f6d1a64f733944ad46b55/helix/01-APPLE-8DVPHAPPA-APPMQC43ID-A-Gold1.jpg",
              altText: "Gold",
              stock: 100,
            },
            {
              id: 104,
              name: "Purple",
              hexCode: "#817688",
              image:
                "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/25976fbb8f069a6e2e05c1ae7c1380eb/helix/01-APPLE-8DVPHAPPA-APPMQC53ID-A-Deep%20Purple1.jpg",
              altText: "Purple",
              stock: 100,
            },
          ],
        },
        {
          name: "iPhone 14 Pro Max 1 TB",
          price: 31999000,
          stok: 100,
          imageDefault: "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/25976fbb8f069a6e2e05c1ae7c1380eb/helix/01-APPLE-8DVPHAPPA-APPMQC53ID-A-Deep%20Purple1.jpg",
          id: 4,
          colors: [
            {
              id: 101,
              name: "Grey",
              hexCode: "#403E3D",
              image:
                "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/eb9131cee70da1c0a2e42acb2d53c127/helix/01-APPLE-8DVPHAPPA-APPMQC23ID-A-Space%20Black1.jpg",
              altText: "Grey",
              stock: 100,
            },
            {
              id: 102,
              name: "Silver",
              hexCode: "#E3E3E5",
              image:
                "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/0fd984c34049b3b308520a4388c931b6/helix/01-APPLE-8DVPHAPPA-APPMQC33ID-A-Silver1.jpg",
              altText: "Silver",
              stock: 100,
            },
            {
              id: 103,
              name: "Gold",
              hexCode: "#FAE7D0",
              image:
                "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/aa8850cf144f6d1a64f733944ad46b55/helix/01-APPLE-8DVPHAPPA-APPMQC43ID-A-Gold1.jpg",
              altText: "Gold",
              stock: 100,
            },
            {
              id: 104,
              name: "Purple",
              hexCode: "#817688",
              image:
                "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/25976fbb8f069a6e2e05c1ae7c1380eb/helix/01-APPLE-8DVPHAPPA-APPMQC53ID-A-Deep%20Purple1.jpg",
              altText: "Purple",
              stock: 100,
            },
          ],
        },
      ],
    };
  },
  computed: {

  }
};
</script>
<style></style>
