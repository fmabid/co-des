<template>
  <div class='gallery-body flex flex-col'>
    <div class='flex flex-row justify-between capitalize px-2 mb-2'>
      <ul class='flex space-x-5 list-none inline'>
        <li>all</li>
        <li>photos</li>
        <li>videos</li>
        <li>freebies</li>
        <li>360</li>
      </ul>

      <div class='dropdown'>
        <div class='flex flex-row items-center space-x-1 cursor-pointer'>
          <p class='flex-auto'>recommended</p>
          <svg id="Group_214" data-name="Group 214" xmlns="http://www.w3.org/2000/svg" width="8" height="4" viewBox="0 0 8 4">
            <g id="Group_58" data-name="Group 58">
              <path id="Path_297" data-name="Path 297" d="M284.091,242.581l4,4,4-4Z" transform="translate(-284.091 -242.581)" fill="#333"/>
            </g>
          </svg>
        </div>

        <div class="dropdown-content">
          <a href="#">Most Recent</a>
          <a href="#">Most Viewed</a>
          <a href="#">Most Downloaded</a>
          <a href='#'>Most Appreciated</a>
        </div>
      </div>
    </div>

    <div class='picture-gallery w-full'>
      <img src='https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885__340.jpg' alt="" class="rounded inset-0 w-full h-full object-cover mb-4" />
      <img src='https://www.w3schools.com/w3css/img_forest.jpg' alt="" class="rounded inset-0 w-full h-full object-cover mb-4" />
      <img src='https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885__340.jpg' alt="" class="rounded inset-0 w-full h-full object-cover mb-4" />

      <Post v-for='index in 51'
            :src='getImage(index)'
            :key='index'/>

      <img src='https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885__340.jpg' alt="" class="rounded inset-0 w-full h-full object-cover mb-4" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'Gallery',
  data() {
    return {
      imgSrc: 'https://source.unsplash.com/random',
      picsum: 'https://picsum.photos/200/300'
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

<style scoped>
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

.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  right: 0;
  background-color: #f9f9f9;
  min-width: 182px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

.dropdown-content a {
  font-size: 16px;
  text-align: right;
  color: black;
  padding: 5px 16px;
  text-decoration: none;
  display: block;
}

.dropdown-content a:hover {background-color: #e8e8e8;}

.dropdown:hover .dropdown-content {
  display: block;
}

</style>
