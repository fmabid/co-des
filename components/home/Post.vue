<template>
  <div class='wrapper relative block'>
    <img :src='src' alt="" class="inset-0 w-full h-full object-cover mb-4 rounded" />
    <div class='overlay flex flex-col justify-between'>
      <div class='flex flex-row justify-end space-x-2'>
        <span class='cursor-pointer'>
          <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 30 30">
            <g id="Group_224" data-name="Group 224" transform="translate(-1338 -1515)">
              <rect id="Rectangle_7697" data-name="Rectangle 7697" width="30" height="30" rx="15" transform="translate(1338 1515)" fill="#fff" opacity="0.8"/>
              <path id="Path_706" data-name="Path 706" d="M50.143,56.635c-3.272-2.433-5.3.824-5.643,1.441-.344-.617-2.371-3.874-5.643-1.441-1.092.812-2.863,4.371,1.077,7.635.946.784,2.914,2.149,3.94,3.176a4.656,4.656,0,0,1,.59.675c.012.017.023.035.035.052.012-.017.023-.035.035-.052a4.661,4.661,0,0,1,.592-.677c1.027-1.026,2.993-2.391,3.939-3.174C53.006,61.007,51.235,57.447,50.143,56.635Z" transform="translate(1308.5 1468.123)" fill="#636363"/>
            </g>
          </svg>
        </span>

        <span class='cursor-pointer'>
          <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 30 30">
            <g id="Group_226" data-name="Group 226" transform="translate(-1375 -1515)">
              <rect id="Rectangle_7698" data-name="Rectangle 7698" width="30" height="30" rx="15" transform="translate(1375 1515)" fill="#fff" opacity="0.8"/>
              <g id="Group_225" data-name="Group 225">
                <rect id="Rectangle_7699" data-name="Rectangle 7699" width="2" height="14" transform="translate(1389 1523)" fill="#636363"/>
                <rect id="Rectangle_7700" data-name="Rectangle 7700" width="2" height="14" transform="translate(1397 1529) rotate(90)" fill="#636363"/>
              </g>
            </g>
          </svg>

        </span>
      </div>

      <div class='flex flex-row justify-between space-x-2'>
        <div class='text-white'>
          <p class="flex items-center text-sm font-medium">
            <img src="https://www.w3schools.com/w3css/img_forest.jpg"
                 alt=""
                 class="w-6 h-6 rounded-full mr-2 bg-gray-100 user border-2">
            Abid
          </p>
        </div>

        <div>
          <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 40 40">
            <g id="Group_288" data-name="Group 288" transform="translate(-1389 -1515)">
              <rect id="Rectangle_7698" data-name="Rectangle 7698" width="40" height="40" rx="20" transform="translate(1389 1515)" fill="#1daf30"/>
              <g id="Group_227" data-name="Group 227" transform="translate(1403.972 1528)">
                <path id="Path_707" data-name="Path 707" d="M1635.222,1002.333l4.145,3.724a.815.815,0,0,0,.544.2h0a.819.819,0,0,0,.543-.2l4.185-3.691a.636.636,0,0,0,.005-.971l-.121-.108a.817.817,0,0,0-.545-.2h0a.818.818,0,0,0-.543.2l-2.541,2.24v-7.844a.98.98,0,0,0-1.947,0v7.83l-2.509-2.254a.817.817,0,0,0-.545-.2h0a.817.817,0,0,0-.543.2l-.122.107A.635.635,0,0,0,1635.222,1002.333Z" transform="translate(-1634.984 -994.815)" fill="#fff"/>
                <path id="Path_708" data-name="Path 708" d="M1643.142,1785.445h-8.4a.745.745,0,0,0-.746.739v.431a.745.745,0,0,0,.746.739h8.4a.745.745,0,0,0,.746-.739v-.431A.745.745,0,0,0,1643.142,1785.445Z" transform="translate(-1634 -1773.353)" fill="#fff"/>
              </g>
            </g>
          </svg>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Post',
  props: {
    src: {
      default: '',
    }
  }
}
</script>

<style scoped>
.overlay {
  display: none;
  width: 100%;
  height: 100%;
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;
  padding: 15px 22px;
}

.wrapper:hover .overlay{
  display: flex;
}

.user{
  width: 40px;
  height: 40px;
}
</style>
