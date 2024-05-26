<template>
    <div class="about-page">
      <h1>About Shopee</h1>
      <section class="intro">
        <p>Welcome to Shopee, your ultimate destination for a diverse range of products. At Shopee, we are committed to bringing you a seamless shopping experience, featuring high-quality items across various categories. Whether you're looking for the latest gadgets or fashionable apparel, Shopee has it all.</p>
      </section>
      
      <section class="categories">
        <h2>Our Categories</h2>
        <ul>
          <li>Mobile</li>
          <li>Tshirt</li>
          <li>Tablet</li>
        </ul>
      </section>
      
      <section class="mission">
        <h2>Our Mission</h2>
        <p>At Shopee, our mission is to provide our customers with a wide variety of products at competitive prices, all while ensuring an enjoyable and hassle-free shopping experience. We carefully curate our product selection to meet the diverse needs and preferences of our shoppers.</p>
      </section>
  
      <section class="commitment">
        <h2>Our Commitment to Quality</h2>
        <p>We prioritize quality in every product we offer. Our dedicated team works tirelessly to source the best items, ensuring that each product meets our high standards of excellence. With Shopee, you can shop with confidence, knowing that quality is guaranteed.</p>
      </section>
      
      <section class="customer-service">
        <h2>Exceptional Customer Service</h2>
        <p>Customer satisfaction is our top priority. Our support team is always ready to assist you with any questions or concerns. We strive to make your shopping experience as smooth and enjoyable as possible, from browsing to delivery.</p>
      </section>
    </div>
  </template>
  
  <script setup>
  import Yourlayout from '@/Layouts/Yourlayout.vue';
  
  defineOptions({
    layout: Yourlayout
  });
  </script>
  
  <style scoped>
  .about-page {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
    font-family: Arial, sans-serif;
    color: white;
  }
  
  h1 {
    text-align: center;
    margin-bottom: 20px;
    font-size: 2.5em;
  }
  
  section {
    margin-bottom: 30px;
  }
  
  h2 {
    font-size: 1.8em;
    margin-bottom: 10px;
  }
  
  p {
    font-size: 1.1em;
    line-height: 1.6;
  }
  
  ul {
    list-style-type: none;
    padding: 0;
  }
  
  ul li {
    background: #ebbebe;
    margin: 5px 0;
    padding: 10px;
    border-radius: 5px;
    color: black;
  }
  </style>
  