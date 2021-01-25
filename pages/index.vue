<template>
  <div class='h-full'>
    <Navbar />

    <div class='relative h-full mx-4 lg:mx-10'>
      <div class='banner flex flex-col align-middle items-center'>
        <p class='title text-3xl w-10/12 lg:w-1/2 lg:px-8 mt-40 md:mt-52 lg:mt-52 pb-4'>
          Your local source of high quality images
          and videos directly from their creators
        </p>

        <div class="flex flex-row bg-white w-10/12 lg:w-1/2 items-center rounded-full pl-2 pr-4 py-1">
          <input type="text"
                 placeholder="Search photos and videos"
                 class="focus:outline-none focus:border-blue-300 rounded-l-full flex-auto py-2 px-2" />

          <svg id="search" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 20 20">
            <g id="Group_93" data-name="Group 93">
              <path id="Path_366" data-name="Path 366" d="M19.878,18.7l-5.81-5.81a7.932,7.932,0,1,0-1.178,1.178l5.81,5.81a.417.417,0,0,0,.589,0l.589-.589A.417.417,0,0,0,19.878,18.7ZM7.917,14.167a6.25,6.25,0,1,1,6.25-6.25A6.257,6.257,0,0,1,7.917,14.167Z" transform="translate(0 0)" fill="#333"/>
            </g>
          </svg>
        </div>

        <p class='w-10/12 lg:w-1/2 lg:px-8 text-gray-400'>
          <span class='text-white'>Recommended:</span> summer, food, covid-19, real estate, love
        </p>

      </div>

      <div class='body-wrapper'>
        <div class='container mx-auto lg:-mt-16 p-8 bg-white'>
          <div class='block mb-4'>
            <p class='text-left text-lg font-bold mb-2'>Top Categories</p>

            <div class='flex-auto flex flex-row space-x-4 justify-between overflow-x-scroll'>
              <Category v-for='idx in 54'
                        :cat-name='`Category ${idx}`'
                        :key='idx' />
            </div>
          </div>

          <Gallery />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

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
</style>
