<template>
  <div>
    <div class="container mx-0 px-0">
      <Navbar />
      <Banner />
      <ProductHomePage />
      <Guarantee />
      <button 
        class="fixed right-[30px] bottom-[20px] text-[#0CDE77] text-6xl hover:scale-150 m-0"
      >
        <i class="fa-brands fa-whatsapp"></i>
      </button>
      <Footer />
    </div>
  </div>
</template>

<script>
export default {
  name: "HomePage",
};
</script>
