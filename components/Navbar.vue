<template>
  <nav class="flex flex-col justify-center fixed w-full top-nav relative">
    <div class="flex items-center justify-between mx-4 lg:mx-10">
      <a href="/">
        <Logo />
      </a>

      <div class="flex items-center justify-between nav-options-container">
        <ul class="flex items-center space-x-5">
          <li class='hover:text-black cursor-pointer'>Explore</li>
          <li class='hover:text-black cursor-pointer'>Discover</li>
          <li class='hover:text-black cursor-pointer'>For Professionals</li>
          <li class='cursor-pointer'>
            <svg xmlns="http://www.w3.org/2000/svg" width="18" height="4" viewBox="0 0 18 4">
              <g id="Group_290" data-name="Group 290" transform="translate(-1199 -31)">
                <circle id="Ellipse_34" data-name="Ellipse 34" cx="2" cy="2" r="2" transform="translate(1213 31)" fill="#818181"/>
                <circle id="Ellipse_35" data-name="Ellipse 35" cx="2" cy="2" r="2" transform="translate(1206 31)" fill="#818181"/>
                <circle id="Ellipse_36" data-name="Ellipse 36" cx="2" cy="2" r="2" transform="translate(1199 31)" fill="#818181"/>
              </g>
            </svg>
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

</style>
