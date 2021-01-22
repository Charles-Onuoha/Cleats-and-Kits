<template>
<div>
    <b-container>
      <b-row>
        <b-col cols="0"> </b-col>
        <!--<div class="col-xs-2 col-sm-3 col-md-4 col-lg-3">-->
        <b-col cols="12 " class="card-row">
          <b-row>
              <!--<div class="col-lg-12">-->
            <b-col v-for="(val, index) in image" :key="index" cols="3">
                <b-card :img-src="getImgUrl(val)" img-alt="Card image" img-top>
              </b-card><br>
              <b-card-text class="text">
                  <h5 class="text-center">{{ header[index] }}</h5>
                  <h5 class="text-center">{{link[index]}}</h5>
                  <b><p class="text-center">
                   &#8358; {{ para[index] }}
                  </p></b>
                </b-card-text>
           <!--  </router-link> -->
            </b-col>
            <!--</div>-->
          </b-row>
        </b-col>
        <!--</div>-->
        <b-col cols="2"> </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
    name: "Bodyy",
    data () {
    return {
      link: [
        'Barcelona Home Jersey',
        'PSG Home Jersey',
        'Real Madrid Home Jersey',
        'Ajax Away Jersey',
        'Chelsea Home Jersey',
        'Juventus Home Jersey',
        'Man United Home Jersey',
        
        

      ],
      header: [
        '20/21 Nike',
        '20/21 Nike',
        '20/21 Adidas',
        '20/21 Adidas',
        '20/21 Nike',
        '20/21 Adidas',
        '20/21 Adidas',
        
      ],
      para: [
        '7000',
        '7000',
        '7000',
        '7000',
        '7000',
        '7000',
        '7000',
        
      ],
      image: ['Barcelona Jersey', 'psg jersey', 'Madrid Jersey', 'Ajax Away', 'Chelsea Jersey', 'Juve Jersey', 'United-Jersey']
    }
  },
  methods: {
    getImgUrl (image) {
      var images = require.context('../assets/images/', false, /\.jpg$/)
      return images('./' + image + '.jpg')
      
    }
  }
}
</script>

<style scoped>
.card {
    position: relative;
    color: black;
    text-decoration: none;
    transition: 0.5s;
    height: 18rem;
    
}

.row {
    margin-top: 1rem;
    line-height: 1.5rem;
}

.card:hover {
    transform: scale(1.1);
}

</style>