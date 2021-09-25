<template>
  <div id="app">
    <h1>shinabitanori-gallery</h1>
    <div>
      <p>小峰さちこ｜shinabitanoriの短歌などの画像</p>
    </div>
    <vue-masonry-gallery
      :imgsArr="media"
      :random="true"
      :target="blank"
      :perPage="18"
      :maxCols="6"
      :loadingTimeOut="100"
    ></vue-masonry-gallery>
  </div>
</template>

<script>
import  VueMasonryGallery from "vue-masonry-gallery";

export default {
  name: 'app',
  components: {
    VueMasonryGallery
  },
  computed: {
    media: () => {
      const imgNames = [
        "14845509871320.jpg_001.jpg",
        "14867833041700.jpg_001.jpg",
        "14885390330400.jpg_001.jpg",
        "14885390707951.jpg_001.jpg",
        "14963935789140.jpg_001.jpg",
        "14986352971381.jpg_001.jpg",
        "14992474318580.jpg_001.jpg",
        "15063428488070.jpg_001.jpg",
        "15093595265920.jpg_001.jpg",
        "15096786015860.jpg_001.jpg",
        "15098563919650.jpg_001.jpg",
        "15117170148770.jpg_001.jpg",
        "15142741510380.jpg_001.jpg",
        "IMG_-kayuzx.jpg_001.jpg",
        "IMG_160t7r.jpg",
        "IMG_20170210_172151.jpg",
        "IMG_20170513_212307.jpg",
        "IMG_20170613_161213.jpg",
        "IMG_20170828_102057.jpg",
        "IMG_20180716_211512.jpg",
        "IMG_20190429_120441.jpg",
        "IMG_20190429_120924.jpg",
        "IMG_20190429_120931.jpg",
        "IMG_20190429_120943.jpg",
        "IMG_20190429_121029.jpg",
        "IMG_20190429_121034.jpg",
        "IMG_20190429_121125.jpg",
        "IMG_20190611_205144.jpg",
        "IMG_ckh2p8.jpg_001.jpg",
        "IMG_xxvnf2.jpg",
        "picture_pc_031feeada78af7d9e5f08a8c13f5e2df.jpg",
        "picture_pc_43eeaf8c101c370115e286bc52aa2366.jpg",
        "picture_pc_5f053b23ab9e873e7b5fc8ea75952d46.jpg",
        "picture_pc_621e20282bdad5bb36047bb2282e392b.jpg",
        "picture_pc_883cc163476201ebc4af455fc59d6923-01.jpeg_001.jpg",
        "picture_pc_883cc163476201ebc4af455fc59d6923.jpg",
        "picture_pc_ccc56936fbdc10a6e5cb5b490f258ba6.jpg",
        "picture_pc_f3eedccd873ac5e24077cdd4cb9a2d3f.jpg",
        "Screenmemo_2016-08-13-18-49-07.jpg",
        "Screenmemo_2016-09-11-21-42-10.jpg",
        "Screenmemo_2016-12-07-17-25-31.jpg",
        "Screenmemo_2016-12-07-17-26-20.jpg",
        "Screenmemo_2016-12-25-06-43-48.jpg",
        "Screenmemo_2017-01-16-16-16-06.jpg",
        "Screenmemo_2017-01-27-04-46-03.jpg",
        "Screenmemo_2017-01-27-04-46-36.jpg",
        "Screenmemo_2017-02-08-19-14-08.jpg",
        "Screenmemo_2017-02-11-12-18-19.jpg",
        "Screenmemo_2017-03-03-20-03-16.jpg",
        "Screenmemo_2017-03-03-20-04-01.jpg",
        "Screenmemo_2017-03-18-18-41-28.jpg",
        "Screenmemo_2017-03-24-11-58-29.jpg",
        "Screenmemo_2017-04-04-17-43-51.jpg",
        "Screenmemo_2017-04-07-19-24-41.jpg",
        "Screenmemo_2017-04-13-19-01-29.jpg",
        "Screenmemo_2017-05-04-10-43-53.jpg",
        "Screenmemo_2017-06-28-16-33-20.jpg",
        "Screenmemo_2017-07-05-18-36-22.jpg",
        "Screenmemo_2017-08-27-03-58-27.jpg",
        "Screenmemo_2017-08-27-04-00-11.jpg",
        "Screenmemo_2017-09-08-23-45-31.jpg",
        "Screenmemo_2017-09-16-00-02-25.jpg",
        "Screenmemo_2017-09-25-21-33-50.jpg",
        "Screenmemo_2017-10-30-19-31-19.jpg",
        "Screenmemo_2017-11-03-12-09-44.jpg",
        "Screenmemo_2017-11-27-02-23-19.jpg",
        "Screenmemo_2017-12-17-10-42-24.jpg",
        "Screenmemo_2017-12-17-10-42-56.jpg",
        "Screenmemo_2017-12-17-10-43-14.jpg",
        "Screenmemo_2017-12-26-16-41-00.jpg",
        "Screenmemo_2017-12-29-20-12-18.jpg",
        "Screenmemo_2018-01-11-18-58-18.jpg",
        "Screenmemo_2018-01-21-18-12-22.jpg",
        "Screenmemo_2018-03-25-11-38-42.jpg",
        "Screenmemo_2018-04-04-12-53-51.jpg",
        "Screenmemo_2018-05-26-19-19-19.jpg",
        "Screenmemo_2018-05-27-11-32-56.jpg",
        "Screenmemo_2018-05-27-12-53-06.jpg",
        "Screenmemo_2018-06-04-18-17-12.jpg",
        "Screenmemo_2018-06-04-21-11-02.jpg",
        "Screenmemo_2018-06-08-02-08-55.jpg",
        "Screenmemo_2018-06-27-19-54-49.jpg",
        "Screenmemo_2018-06-27-19-55-33.jpg",
        "Screenmemo_2018-06-27-19-56-18.jpg",
        "Screenmemo_2018-06-27-19-57-31.jpg",
        "Screenmemo_2018-07-01-09-17-44.jpg",
        "Screenmemo_2018-07-07-22-21-27.jpg",
        "Screenmemo_2018-07-28-12-08-54.jpg",
        "Screenmemo_2018-10-21-20-27-25.jpg",
        "Screenmemo_2018-11-04-16-05-38.jpg",
        "Screenmemo_2018-11-19-20-19-34.jpg",
        "up_5825cbcb1b95d2f6e5b466430042da9d.jpg",
        "up_c9e7b60e874f92e50c1beeb6f3d81132.jpg",
        "up_faa39e5572097812ca3a7356a1862f39_275.jpg"
      ]
      return imgNames.map(el => {
        return {
          href: `https://rawcdn.githack.com/paithiov909/gallery/ced203819e01a61b3e931facdc5d5fc8987d8446/images/${el}`,
          src: `https://rawcdn.githack.com/paithiov909/gallery/ced203819e01a61b3e931facdc5d5fc8987d8446/images/${el}`,
        }
      })
    }
  }
}
</script>

<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  height: 100vh;
}
</style>
