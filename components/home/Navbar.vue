<template>
  <nav class="flex flex-col justify-center fixed w-full top-nav relative">
    <div class="flex items-center justify-between mx-4 lg:mx-10">
      <a href='/'>
        <Logo />
      </a>

      <div class="block lg:hidden">
        <button class="flex items-center px-3 py-2 border rounded text-black border-black">
          <svg
            class="fill-current h-3 w-3"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <title>Menu</title>
            <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" />
          </svg>
        </button>
      </div>

      <div class="lg:flex hidden items-center justify-between nav-options-container">
        <ul class="flex items-center space-x-5">
          <li class='hover:text-black cursor-pointer'>Explore</li>
          <li class='hover:text-black cursor-pointer'>Discover</li>
          <li class='hover:text-black cursor-pointer'>For Professionals</li>
          <li class='cursor-pointer'>
            <div class="dropdown">
              <div class='py-7 px-2'>
                <svg xmlns="http://www.w3.org/2000/svg" width="18" height="4" viewBox="0 0 18 4">
                  <g id="Group_290" data-name="Group 290" transform="translate(-1199 -31)">
                    <circle id="Ellipse_34" data-name="Ellipse 34" cx="2" cy="2" r="2" transform="translate(1213 31)" fill="#818181"/>
                    <circle id="Ellipse_35" data-name="Ellipse 35" cx="2" cy="2" r="2" transform="translate(1206 31)" fill="#818181"/>
                    <circle id="Ellipse_36" data-name="Ellipse 36" cx="2" cy="2" r="2" transform="translate(1199 31)" fill="#818181"/>
                  </g>
                </svg>
              </div>

              <div class="dropdown-content divide-y divide-gray-800">
                <div>
                  <a href="#">About Click Motto</a>
                  <a href="#">Pricing</a>
                  <a href="#">License</a>
                  <a href="#">Partnerships</a>
                  <a href="#">Blog</a>
                  <a href="#">Help</a>
                  <a href="#">Join The Team</a>
                  <a href="#">Link</a>
                </div>

                <div class='icons px-4'>
                  <ul class='flex flex-row justify-between'>
                    <li>
                      <a href='#'>
                        <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 18 18">
                          <path id="Path_717" data-name="Path 717" d="M8.966,18h0Zm.064,0h0Zm-.091,0h0Zm.12,0h0Zm-.146,0h0Zm.175,0h0Zm.029,0h0Zm-.239,0h0Zm.267,0h0Zm-.3,0h0Zm.325,0h0Zm-.351,0h0ZM8.79,18h0ZM9.2,18h0Zm-.442,0h0Zm.471,0h0Zm.029,0h0Zm-.526,0h0ZM8.71,18h0Zm.58,0h0Zm.029,0h0Zm-.646,0h0Zm-.026,0h0Zm.7,0h0Zm-.727,0h0Zm.755,0h0Zm-.792,0h0Zm.821,0h0Zm-.847,0h0Zm.876,0h0Zm-.9,0h0Zm.93,0h0Zm.029,0h0Zm-.982,0h0Zm1.01,0h0Zm-1.049,0h0Zm-.025,0h0Zm1.1,0h0Zm-1.128,0h0Zm1.157,0h0Zm.029,0h0Zm-1.222,0h0Zm-.025,0h0Zm1.276,0h0Zm-1.3,0h0Zm1.329,0h0Zm-1.364,0h0Zm1.392,0h0Zm.029,0h0Zm-1.447,0h0Zm-.026,0h0Zm1.5,0h0Zm-1.529,0h0Zm1.558,0Zm.029,0h0Zm-1.616,0h0Zm-.026,0h0Zm1.671,0h0Zm-2.24-.071a9,9,0,1,1,2.813,0V11.6h2.1L12.9,9h-2.5V7.312a1.3,1.3,0,0,1,1.466-1.406h1.135V3.691a13.862,13.862,0,0,0-2.015-.175,3.176,3.176,0,0,0-3.4,3.5V9H5.309v2.6H7.594Z" fill="#e17800" fill-rule="evenodd"/>
                        </svg>
                      </a>
                    </li>
                    <li>
                      <a href='#'>
                        <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 18 18">
                          <path id="Path_718" data-name="Path 718" d="M9,0A9,9,0,1,1,0,9,9,9,0,0,1,9,0ZM7.415,13.787a6.119,6.119,0,0,0,6.16-6.161c0-.094,0-.188,0-.278a4.425,4.425,0,0,0,1.082-1.122,4.4,4.4,0,0,1-1.244.341,2.164,2.164,0,0,0,.952-1.2,4.373,4.373,0,0,1-1.374.525A2.166,2.166,0,0,0,9.242,7.375a1.976,1.976,0,0,0,.058.494A6.14,6.14,0,0,1,4.838,5.606a2.164,2.164,0,0,0,.673,2.887,2.131,2.131,0,0,1-.979-.269v.027A2.167,2.167,0,0,0,6.27,10.374a2.15,2.15,0,0,1-.57.076,2.066,2.066,0,0,1-.409-.04,2.162,2.162,0,0,0,2.021,1.5,4.351,4.351,0,0,1-2.689.925,3.929,3.929,0,0,1-.516-.031A6.035,6.035,0,0,0,7.415,13.787Z" fill="#e17800" fill-rule="evenodd"/>
                        </svg>
                      </a>
                    </li>
                    <li>
                      <a href='#'>
                        <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 18 18">
                          <path id="Path_720" data-name="Path 720" d="M9,0A9,9,0,1,1,0,9,9,9,0,0,1,9,0ZM9,3.375c-1.528,0-1.719.006-2.319.034a4.137,4.137,0,0,0-1.365.262A2.872,2.872,0,0,0,3.67,5.316a4.137,4.137,0,0,0-.262,1.365c-.028.6-.034.791-.034,2.319s.006,1.719.034,2.319a4.137,4.137,0,0,0,.262,1.365A2.872,2.872,0,0,0,5.316,14.33a4.137,4.137,0,0,0,1.365.262c.6.028.791.034,2.319.034s1.719-.006,2.319-.034a4.137,4.137,0,0,0,1.365-.262,2.872,2.872,0,0,0,1.645-1.645,4.137,4.137,0,0,0,.262-1.365c.028-.6.034-.791.034-2.319s-.006-1.719-.034-2.319a4.137,4.137,0,0,0-.262-1.365A2.872,2.872,0,0,0,12.684,3.67a4.137,4.137,0,0,0-1.365-.262C10.719,3.381,10.528,3.375,9,3.375ZM9,4.389c1.5,0,1.68.006,2.273.033a3.138,3.138,0,0,1,1.045.194,1.866,1.866,0,0,1,1.068,1.068,3.138,3.138,0,0,1,.193,1.045c.027.593.033.771.033,2.273s-.006,1.68-.033,2.273a3.138,3.138,0,0,1-.193,1.045,1.871,1.871,0,0,1-1.068,1.068,3.138,3.138,0,0,1-1.045.193c-.593.027-.771.033-2.273.033s-1.68-.006-2.273-.033a3.138,3.138,0,0,1-1.045-.193,1.866,1.866,0,0,1-1.068-1.068,3.138,3.138,0,0,1-.194-1.045C4.394,10.68,4.389,10.5,4.389,9s.006-1.68.033-2.273a3.138,3.138,0,0,1,.194-1.045A1.866,1.866,0,0,1,5.682,4.615a3.138,3.138,0,0,1,1.045-.194C7.32,4.394,7.5,4.389,9,4.389ZM9,6.112A2.888,2.888,0,1,0,11.888,9,2.888,2.888,0,0,0,9,6.112Zm0,4.763A1.875,1.875,0,1,1,10.875,9,1.875,1.875,0,0,1,9,10.875ZM12.678,6A.675.675,0,1,1,12,5.322.675.675,0,0,1,12.678,6Z" fill="#e17800" fill-rule="evenodd"/>
                        </svg>
                      </a>
                    </li>
                    <li>
                      <a href='#'>
                        <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 18 18">
                          <path id="Path_721" data-name="Path 721" d="M9,0A9,9,0,0,0,5.72,17.383,8.643,8.643,0,0,1,5.752,14.8c.163-.7,1.055-4.474,1.055-4.474a3.245,3.245,0,0,1-.269-1.336c0-1.252.726-2.186,1.628-2.186A1.131,1.131,0,0,1,9.3,8.071a18.128,18.128,0,0,1-.745,3,1.307,1.307,0,0,0,1.333,1.627c1.6,0,2.829-1.687,2.829-4.121a3.553,3.553,0,0,0-3.76-3.662A3.9,3.9,0,0,0,4.9,8.817a3.5,3.5,0,0,0,.669,2.054.269.269,0,0,1,.062.258c-.068.285-.22.9-.25,1.021-.039.165-.13.2-.3.12A4.036,4.036,0,0,1,3.252,8.783c0-2.839,2.063-5.446,5.947-5.446a5.282,5.282,0,0,1,5.549,5.2c0,3.1-1.956,5.6-4.67,5.6A2.41,2.41,0,0,1,8.014,13.1s-.451,1.718-.561,2.139A10.046,10.046,0,0,1,6.335,17.6,9,9,0,1,0,9,0Z" fill="#e17800"/>
                        </svg>
                      </a>
                    </li>
                    <li>
                      <a href='#'>
                        <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 18 18">
                          <path id="Path_722" data-name="Path 722" d="M9,0A9,9,0,1,1,0,9,9,9,0,0,1,9,0Zm5.035,7.236q-.07,1.54-2.151,4.217-2.151,2.794-3.639,2.8-.922,0-1.56-1.7-.425-1.56-.851-3.121-.473-1.7-1.016-1.7a3.257,3.257,0,0,0-.828.5l-.5-.639q.781-.686,1.539-1.372A3.484,3.484,0,0,1,6.6,5.26q1.231-.119,1.515,1.683.307,1.943.426,2.417.355,1.612.781,1.612.331,0,.994-1.046a4.111,4.111,0,0,0,.71-1.592q.1-.9-.71-.9a1.981,1.981,0,0,0-.781.173q.778-2.546,2.971-2.475Q14.129,5.176,14.035,7.236Z" fill="#e17800" fill-rule="evenodd"/>
                        </svg>
                      </a>
                    </li>
                    <li>
                      <a href='#'>
                        <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 18 18">
                          <path id="Path_723" data-name="Path 723" d="M9,0A9,9,0,1,1,0,9,9,9,0,0,1,9,0Zm5.254,13.743v-.177l-.822-.807a.246.246,0,0,1-.093-.236V6.591a.246.246,0,0,1,.093-.236l.842-.807V5.37H11.359L9.281,10.554,6.917,5.37H3.859v.177l.985,1.186a.407.407,0,0,1,.133.345V11.74a.536.536,0,0,1-.142.462L3.727,13.546v.177H6.868v-.177L5.76,12.2a.555.555,0,0,1-.152-.462V7.709l2.757,6.015h.32l2.368-6.015V12.5c0,.128,0,.152-.084.236l-.852.827v.177Z" fill="#e17800" fill-rule="evenodd"/>
                        </svg>
                      </a>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </li>
          <li class='cursor-pointer'>
            <button class="btn text-center border border-gray-300" type='button'>Submit Photos</button>
          </li>
        </ul>

        <div class="separator-y mr-8 ml-4" />
        <p class="mr-4 cursor-pointer">
          Login
        </p>

        <div class="flex">
          <button class="btn text-center btn-join" type='button'>Button A</button>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style scoped>
nav {
  z-index: 100;
  color: #818181;
  font-size: 15px;
}
.top-nav {
  height: 64px;
}

.nav-options-container {
  width: auto;
}

.nav-options img {
  margin: 0 12px;
  cursor: pointer;
}

.separator-y {
  width: 1px;
  height: 32px;
  background-color: #dfe0eb;
}

.btn{
  border-radius: 6px;
  padding: 4px 14px;
}

.btn-join{
  color: white;
  background: #e17800;
}


.dropdown {
  float: left;
  overflow: hidden;
}

.dropdown-content {
  display: none;
  position: absolute;
  color: #929292;
  font-size: 15px;
  background-color: #111;
  min-width: 218px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

.dropdown-content a {
  float: none;
  color: #929292;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
  text-align: left;
}

.dropdown-content a:hover {
  background-color: #1c1c1c;
  color: white;
}

.dropdown:hover .dropdown-content {
  display: block;
}


.icons ul li a{
  padding: 12px 0;
}

.icons ul li a:hover{
  background-color: transparent;
}
</style>
