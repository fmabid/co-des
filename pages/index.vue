<template>
  <div class='h-full'>
    <Navbar />

    <div class='relative h-full mx-4 lg:mx-10'>
      <div class='banner flex flex-col align-middle items-center'>
        <p class='title text-3xl w-1/2 px-8 mt-52'>
          Your local source of high quality images
          and videos directly from their creators
        </p>

        <div class="flex flex-row bg-white w-1/2 items-center rounded-full pl-2 pr-4 py-1">
          <input type="text"
                 placeholder="Search photos and videos"
                 class="focus:outline-none focus:border-blue-300 rounded-l-full flex-auto py-2 px-2" />

          <svg id="search" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 20 20">
            <g id="Group_93" data-name="Group 93">
              <path id="Path_366" data-name="Path 366" d="M19.878,18.7l-5.81-5.81a7.932,7.932,0,1,0-1.178,1.178l5.81,5.81a.417.417,0,0,0,.589,0l.589-.589A.417.417,0,0,0,19.878,18.7ZM7.917,14.167a6.25,6.25,0,1,1,6.25-6.25A6.257,6.257,0,0,1,7.917,14.167Z" transform="translate(0 0)" fill="#333"/>
            </g>
          </svg>
        </div>

      </div>

      <div class='body-wrapper'>
        <div class='container mx-auto -mt-16 p-8 bg-white'>
          <div class='bg-blue-200 mb-4'>
            <p class='text-left text-lg font-bold'>Top Categories</p>
          </div>

          <div class='gallery-body flex flex-col'>
            <div class='flex flex-row justify-between capitalize px-2 mb-2'>
              <ul class='flex space-x-5 list-none inline'>
                <li>all</li>
                <li>photos</li>
                <li>videos</li>
                <li>freebies</li>
                <li>360</li>
              </ul>

              <div class='flex flex-row items-center space-x-1 cursor-pointer'>
                <p class='flex-auto'>recommended</p>
                <svg id="Group_214" data-name="Group 214" xmlns="http://www.w3.org/2000/svg" width="8" height="4" viewBox="0 0 8 4">
                  <g id="Group_58" data-name="Group 58">
                    <path id="Path_297" data-name="Path 297" d="M284.091,242.581l4,4,4-4Z" transform="translate(-284.091 -242.581)" fill="#333"/>
                  </g>
                </svg>
              </div>
            </div>

            <div class='picture-gallery w-full'>
              <Post v-for='index in 11'
                    :src='getImage(index)'
                    :key='index'/>

              <img src='https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885__340.jpg' alt="" class="inset-0 w-full h-full object-cover mb-4" />
              <img src='https://www.w3schools.com/w3css/img_forest.jpg' alt="" class="inset-0 w-full h-full object-cover mb-4" />
              <img src='https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885__340.jpg' alt="" class="inset-0 w-full h-full object-cover mb-4" />
              <img src='https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885__340.jpg' alt="" class="inset-0 w-full h-full object-cover mb-4" />
            </div>
          </div>

<!--          <div class='picture-gallery'>-->
<!--            <img src="https://www.w3schools.com/w3css/img_forest.jpg" alt="" class="absolute inset-0 w-full h-full object-cover" />-->
<!--            <img src="https://source.unsplash.com/random" alt="" class="absolute inset-0 w-full h-full object-cover" />-->
<!--            <img src="https://source.unsplash.com/random" alt="" class="absolute inset-0 w-full h-full object-cover" />-->
<!--          </div>-->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      imgSrc: 'https://source.unsplash.com/random',
      picsum: 'https://picsum.photos/200/200'
    };
  },
  methods: {
    getImage (id){
      if (parseInt(id) % 2 === 0) {
        return this.imgSrc
      } else {
        return this.picsum
      }
    }
  }
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/

body{
  height: 100vh;
}
</style>

<style scoped>
.banner{
  z-index: -1000;
  height: 600px;
  width: 100%;
  background-image: url("https://source.unsplash.com/random");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

.banner .title{
  font-weight: bold;
  color: #fff;
}

.body-wrapper{
  position: relative;
  width: 100%;
  z-index: 500;
  top: 50%;
}

.picture-gallery{
  display: block;
  column-count: 1;
}


@media (min-width: 768px) {
  .picture-gallery {
    column-count: 2;
  }
}

@media (min-width: 992px) {
  .picture-gallery {
    column-count: 3;
  }
}

@media (min-width: 1200px) {
  .picture-gallery {
    column-count: 3;
  }
}

@media (min-width: 1920px) {
  .picture-gallery {
    column-count: 5;
  }
}


</style>
