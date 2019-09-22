<template>
  <div>
    <HomeCarousel/>
<b-container>
<section class="mb-5">
  <h1 class="mb-3">Рекомендуемые предметы</h1>
  <ProductSlider :products="products"/>
  <div class="row">
    <div class="col-2"></div>
    <div class="col-10"></div>
  </div>

</section>
  <section>
    <h1 class="mb-3">Новинки</h1>
    <ProductSlider :products="products"/>
  </section>
</b-container>
  </div>
</template>

<script>

import HomeCarousel from "../components/HomeCarousel";
import ProductSlider from "../components/ProductSlider";

export default {
    name : 'HomePage',
  components: {ProductSlider, HomeCarousel},
  data() {
    return {
      products :[
        {
          id:1,
          title:'Some product 1',
          price : 789,
          image: 'https://picsum.photos/200/200/?image=41'
        },
        {
          id:2,
          title:'Some product 2',
          price : 322,
          image: 'https://picsum.photos/200/200/?image=42'
        },
        {
          id:3,
          title:'Some product 3',
          price : 4078,
          image: 'https://picsum.photos/200/200/?image=43'
        },
        {
          id:4,
          title:'Some product 4',
          price : 210,
          image: 'https://picsum.photos/200/200/?image=44'
        },
        {
          id:5,
          title:'Some product 5',
          price : 400,
          image: 'https://picsum.photos/200/200/?image=45'
        },
        {
          id:6,
          title:'Some product 6',
          price : 530,
          image: 'https://picsum.photos/200/200/?image=46'
        }
      ]
    }

  }
}
</script>
