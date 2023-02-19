<template>
  <div>
    <section>
      <div class="max-w-screen-xl px-4 py-8 mx-auto sm:px-6 sm:py-12 lg:px-8">
        <header>
          <h2 class="text-xl font-bold text-gray-900 sm:text-3xl">
            Product Collection
          </h2>

          <p class="max-w-md mt-4 text-gray-500">
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Itaque
            praesentium cumque iure dicta incidunt est ipsam, officia dolor
            fugit natus?
          </p>
        </header>
        
        <!-- <div class="flex items-center justify-between mt-8">
          <div
            class="flex border border-gray-100 divide-x divide-gray-100 rounded"
          >
            <button
              class="inline-flex items-center justify-center w-10 h-10 text-gray-600 transition hover:bg-gray-50 hover:text-gray-700"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-5 h-5"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M3.75 6A2.25 2.25 0 016 3.75h2.25A2.25 2.25 0 0110.5 6v2.25a2.25 2.25 0 01-2.25 2.25H6a2.25 2.25 0 01-2.25-2.25V6zM3.75 15.75A2.25 2.25 0 016 13.5h2.25a2.25 2.25 0 012.25 2.25V18a2.25 2.25 0 01-2.25 2.25H6A2.25 2.25 0 013.75 18v-2.25zM13.5 6a2.25 2.25 0 012.25-2.25H18A2.25 2.25 0 0120.25 6v2.25A2.25 2.25 0 0118 10.5h-2.25a2.25 2.25 0 01-2.25-2.25V6zM13.5 15.75a2.25 2.25 0 012.25-2.25H18a2.25 2.25 0 012.25 2.25V18A2.25 2.25 0 0118 20.25h-2.25A2.25 2.25 0 0113.5 18v-2.25z"
                />
              </svg>
            </button>

            <button
              class="inline-flex items-center justify-center w-10 h-10 text-gray-600 transition hover:bg-gray-50 hover:text-gray-700"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-5 h-5"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M3.75 5.25h16.5m-16.5 4.5h16.5m-16.5 4.5h16.5m-16.5 4.5h16.5"
                />
              </svg>
            </button>
          </div>

          <div>
            <label for="SortBy" class="sr-only">SortBy</label>

            <select id="SortBy" class="h-10 text-sm border-gray-300 rounded">
              <option>Sort By</option>
              <option value="Title, DESC">Title, DESC</option>
              <option value="Title, ASC">Title, ASC</option>
              <option value="Price, DESC">Price, DESC</option>
              <option value="Price, ASC">Price, ASC</option>
            </select>
          </div>
        </div> -->

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
    </section>
  </div>
</template>
<script>
export default {
    data() {
    return {
      productHomePage: [
        {
          image:
            "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/7eca1fd03f15b186b09bdb5c9a60ac0b/helix/01-APPLE-8DVPHAPPA-APPMQ9P3ID-A-Space%20Black1.jpg",
          name: "iPhone 14 Pro Max",
          price: "20.999.000",
        },
        {
          image:
            "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/0a3a7f87e43a73d920b916e7d3c6e1d6/helix/01-APPLE-8DVLPAPP0-APPMGN63ID-A-SpaceGrayRevSS.jpg",
          name: "MacBook Air M1 2020 13 inch",
          price: "13.999.000",
        },
        {
          image:
            "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/26b725a3e06a7717878aea19573f3940/helix/01-APPLE-8DVWAAPP0-APPLE-WATCH-S8-45-SIL-AL-WT-SP-GPS-IND-Silver.jpg",
          name: "Apple Watch S8",
          price: "6.999.000",
        },
        {
          image:
            "https://bb-scm-prod-pim.oss-ap-southeast-5.aliyuncs.com/products/3d2e443d797bc9fff440a14ae7700efd/helix/01-APPLE-8DVTBAPP0-APPMNYM3PA-A-Silver.jpg",
          name: "iPad Pro 11 inch (2022)",
          price: "15.499.000",
        },
      ],
    };
  },
};
</script>
<style></style>
