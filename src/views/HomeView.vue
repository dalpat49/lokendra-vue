<template>

  <nav class="bg-gray-800">
  <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
    <div class="relative flex h-16 items-center justify-between">
      <div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
        <!-- Mobile menu button-->
        <button type="button" class="relative inline-flex items-center justify-center rounded-md p-2 text-gray-400 hover:bg-gray-700 hover:text-white focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white" aria-controls="mobile-menu" aria-expanded="false">
          <span class="absolute -inset-0.5"></span>
          <span class="sr-only">Open main menu</span>
          <!--
            Icon when menu is closed.

            Menu open: "hidden", Menu closed: "block"
          -->
          <svg class="block h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
          </svg>
          <!--
            Icon when menu is open.

            Menu open: "block", Menu closed: "hidden"
          -->
          <svg class="hidden h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
          </svg>
        </button>
      </div>
      <div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start">
        <div class="flex flex-shrink-0 items-center">
          <img class="h-8 w-auto" src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=500" alt="Your Company">
        </div>
        <div class="hidden sm:ml-6 sm:block">
          <div class="flex space-x-4">
            <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
            <a href="#" class="bg-gray-900 text-white rounded-md px-3 py-2 text-sm font-medium" aria-current="page">Dashboard</a>
            <a href="#second_section" class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md px-3 py-2 text-sm font-medium">About</a>
            <a href="#project" class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md px-3 py-2 text-sm font-medium">Projects</a>
            <a href="#portfolio" class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md px-3 py-2 text-sm font-medium">Calendar</a>
          </div>
        </div>
      </div>
      <div class="absolute inset-y-0 right-0 flex items-center pr-2 sm:static sm:inset-auto sm:ml-6 sm:pr-0">
        <button type="button" class="relative rounded-full bg-gray-800 p-1 text-gray-400 hover:text-white focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800">
          <span class="absolute -inset-1.5"></span>
          <span class="sr-only">View notifications</span>
          <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" d="M14.857 17.082a23.848 23.848 0 005.454-1.31A8.967 8.967 0 0118 9.75v-.7V9A6 6 0 006 9v.75a8.967 8.967 0 01-2.312 6.022c1.733.64 3.56 1.085 5.455 1.31m5.714 0a24.255 24.255 0 01-5.714 0m5.714 0a3 3 0 11-5.714 0" />
          </svg>
        </button>

        <!-- Profile dropdown -->
        <div class="relative ml-3">
          <div>
            <button type="button" class="relative flex rounded-full bg-gray-800 text-sm focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800" id="user-menu-button" aria-expanded="false" aria-haspopup="true">
              <span class="absolute -inset-1.5"></span>
              <span class="sr-only">Open user menu</span>
              <img class="h-8 w-8 rounded-full" src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="">
            </button>
          </div>

          <!--
            Dropdown menu, show/hide based on menu state.

            Entering: "transition ease-out duration-100"
              From: "transform opacity-0 scale-95"
              To: "transform opacity-100 scale-100"
            Leaving: "transition ease-in duration-75"
              From: "transform opacity-100 scale-100"
              To: "transform opacity-0 scale-95"
          -->
          
        </div>
      </div>
    </div>
  </div>

  <!-- Mobile menu, show/hide based on menu state. -->
  <div class="hidden" id="mobile-menu">
    <div class="space-y-1 px-2 pb-3 pt-2">
      <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
      <a href="#" class="bg-gray-900 text-white block rounded-md px-3 py-2 text-base font-medium" aria-current="page">Dashboard</a>
      <a href="#second_section" class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">About</a>
      <a href="#project" class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Projects</a>
      <a href="#portfolio" class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Calendar</a>
    </div>
  </div>
</nav>



  <!-- First_section -->
  <section class="bg-white">
      <div class="relative bg-cover grid lg:grid-cols-2 grid-cols-1 gap-8 items-center interiorDesign " style="height: 400px; background-position: 0% 20%;background-size: cover;">
        <div class="md:flex lg:justify-end mt-56 justify-start sm:block lg:px-0 sm:px-10 px-8">
          <div class="font-sans bg-[#2530c9] lg:absolute md:relative sm:p-8 p-8 sm:py-10 align-bottom shadow-2xl shadow-indigo-500/50 sm:block sm:p-0 sm:py-0">
            <h1 class="sm:text-[3rem] leading-none text-white font-medium text-3xl">Digital Art<br>& Design Studio</h1>
            <p class="lg:w-80 text-white md:text-[1.2rem] text-lg py-6 w-full">Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim</p>
            <a class="px-2 text-white uppercase underline underline-offset-4 	">Learn More</a>
          </div>
        </div>
        <div class="sm:flex sm:mb-24 md:m-4 sm:block lg:px-0 sm:px-10 lg:py-0 px-8">
          <div class="font-sans bg-[#3e427e] lg:absolute sm:p-8 p-8 sm:py-10 align-bottom shadow-2xl shadow-indigo-500/50  sm:block ">
            <h2 class="text-[2.7rem] leading-none text-white font-medium ">Our Mission</h2>
            <p class="lg:w-80 font-normal text-white md:text-[1.4rem] sm:text-lg text-xl py-4 w-full">Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident.</p>
          </div>
        </div>        
      </div>
      <div class="flex justify-center mt-80 py-10 text-lg bg-white shadow-lg xl:pt-20 lg:pt-10  sm:pt-60 pt-96">
            <p class="abcd">Image from <a class="underline underline-offset-8 text-black decoration-[#3e427e] hover:none">Freepik</a></p>
          </div>
  </section>

  <!-- Second section -->
  <section id="second_section" class="bg-[#2530c9] md:flex justify-center block"> 
    <div class="flex relative sm:block">
      <div class="grid md:grid-col-1 lg:grid-cols-2 gap-2 text-white  lg:pl-20 lg:pr-10 sm:pt-10 sm:pl-20 xl:pt-2 sm:pr-10 md:pl-10 pl-8 pr-8 sm:mt-0 mt-10"  >
        <div class="flex align-center items-center sm:pr-16 sm:pr-0 sm:align-start sm:block  md:flex md:align-center md:items-center md:pr-6 md:pl-0 xl:pl-24 xl:pr-20">
          <div>
            <h6 class="text-2xl font-normal pt-2 ">ABOUT COMPANY</h6>
            <h1 class="sm:text-6xl text-4xl font-bold py-4 ">Need Amazing Design?</h1>
            <P class="sm:text-[1.210rem] text-base ">Paragraph. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur id suscipit ex. Suspendisse rhoncus laoreet purus quis elementum. Phasellus sed efficitur dolor, et ultricies sapien. Quisque fringilla sit amet dolor commodo efficitur.Aliquam et sem odio. In ullamcorper nisi nunc, et molestie ipsum iaculis sit amet. </P>
            <p class="bg-[#f49ea8] hover:bg-[#259bca]  text-2xl px-10 py-4 rounded-full absolute font-semibold mt-5 tracking-widest">LEARN MORE</p>
          </div>
        </div>
     

      <div class="md:flex md:space-x-8 lg:py-0 lg:pb-10 py-10">        
        <div class=" mt-36 ">
          <div class="bg-white md:w-full  text-black py-16 px-8 shadow-2xl">
            <div class="md:shrink-0">
              <img src="/src/assets/images/network_icon.png" style="height: 80px; width: 80px;"/>
            </div>
            <div class=" mt-4">
              <h5 class="text-2xl font-medium">Sample Headline</h5>
            </div>
            <div class="mt-4 italic ">
              <p class="text-lg text-neutral-500">Sample text. Click to select the text box. Click again or double click to start editing the text.</p>
            </div>
          </div>
          <div class="bg-white md:w-full text-black py-16 px-8 shadow-2xl mt-5">
            <div class="md:shrink-0">
              <img src="/src/assets/images/suitcase_icon.png" style="height: 80px; width: 80px;"/>
            </div>
            <div class="mt-4">
              <h5 class="text-2xl font-medium">Sample Headline</h5>
            </div>
            <div class="mt-4 italic ">
              <p class="text-lg text-neutral-500">Sample text. Click to select the text box. Click again or double click to start editing the text.</p>
            </div>
          </div>
        </div>
        <div class="mt-6">
          <div class="bg-white md:w-full text-black py-16 px-8 shadow-2xl">
            <div class="md:shrink-0">
              <img src="/src/assets/images/lightbulb_icon.png" style="height: 80px; width: 80px;"/>
            </div>
            <div class="mt-4 ">
              <h5 class="text-2xl font-medium">Sample Headline</h5>
            </div>
            <div class="mt-4 italic ">
              <p class="text-lg text-neutral-500">Sample text. Click to select the text box. Click again or double click to start editing the text.</p>
            </div>
          </div>
          <div class="bg-white md:w-full text-black py-16 px-8 shadow-2xl mt-5">
            <div class="md:shrink-0">
              <img src="/src/assets/images/camera_icon.png" style="height: 80px; width: 80px;"/>
            </div>
            <div class="mt-4">
              <h5 class="text-2xl font-medium">Sample Headline</h5>
            </div>
            <div class="mt-4 italic ">
              <p class="text-lg text-neutral-500">Sample text. Click to select the text box. Click again or double click to start editing the text.</p>
            </div>
          </div>
        </div>
      </div>
      </div>
    </div>
  </section>





    <!-- New Section  -->
    <section>
      <div class="grid lg:grid-cols-2 lg:mt-16 mt-32 mb-10 lg:min-h-[800px] min-h-[900px]">
        <div class="flex relative flex-col justify-center flex-nowrap  lg:min-w-[52rem] sm:pr-0 pr-6">
          <div class="bg-[#f9c9ce] min-h-[190px] flex lg:justify-center-items lg:justify-center justify-end items-center xl:max-w-[880px] lg:max-w-[800px] md:max-w-[800px] sm:max-w-[650px] max-w-[650px] ">     
            <div class="bg-cover bg-center absolute md:min-h-[360px] md:w-[380px] lg:w-[280px] w-[320px] h-[400px] border-4 border-white lg:ml-0 lg:ml-0 lg:mr-[0px] mb-[14px]" style="background-image: url('https://images02.nicepage.com/c461c07a441a5d220e8feb1a/6d35051f156a5a558e14089e/v.jpg?version=;')"></div>            
          </div> 
          <div class="flow self-center xl:pl-10 lg:pl-0 xl:pr-0 lg:pr-20 md:pl-24 lg:mt-10 lg:mt-10">
              <div>
                <p class="text-[#2530c9] font-semibold lg:text-3xl md:text-4xl text-3xl lg:mt-16 mt-32 lg:py-6 py-2">What We Offer:</p>
              </div>
               <div>
                <ul>
                  <li class="flex px-1 pt-1">
                    <i class="fi fi-bs-check text-[#2530c9] text-lg pr-2 pt-1"></i>
                    <p class="text-black text-lg">Duis aute irure dolor in</p>
                  </li>
                  <li class="flex px-1 pt-1">
                    <i class="fi fi-bs-check text-[#2530c9] text-lg pr-2 pt-1"></i>
                    <p class="text-black text-lg">Excepteur sint occaecat</p>
                  </li>
                  <li class="flex px-1 pt-1">
                    <i class="fi fi-bs-check text-[#2530c9] text-lg pr-2 pt-1"></i>
                    <p class="text-black text-lg">Ut enim ad minim</p>
                  </li>
                  <li class="flex px-1 pt-1">
                    <i class="fi fi-bs-check text-[#2530c9] text-lg pr-2 pt-1"></i>
                    <p class="text-black text-lg">Lorem ipsum dolor</p>
                  </li>              
                </ul>
                <div class="mt-4  text-lg text-black">
                  <p>Images from <a class="underline underline-offset-8 text-black cursor-pointer hover:bg-white"> Freepik</a></p>
                </div>
            </div>
          </div>
        </div>  
        
        <!-- 2nd Section -->
        <div class="md:items-center md:flex lg:mt-20 mt-10 flex   lg:justify-start sm:justify-center md:justify-end  sm:pl-0  pl-12">
          <div class="bg-[#2530c9] text-white lg:w-[470px] md:w-[400px] sm:w-[380px] w-[300px] absolute px-8 lg:mx-10 xl:mx-0 lg:py-10 py-4 lg:mr-0 md:mr-60">
            <p class="lg:text-4xl md:text-3xl text-xl font-semibold md:py-4" >BRANDING & DESIGN</p>
            <p class="lg:text-[1.050rem] lg:py-4 py-2 text-small">Quam nulla porttitor massa id neque aliquam vestibulum morbi. Eu consequat ac felis donec et odio pellentesque. Turpis nunc eget lorem dolor sed. Ornare quam viverra orci sagittis eu volutpat odio. Sed vulputate odio ut enim blandit volutpat.</p>
            <p class="lg:py-8 py-4 text-lg">Images from <a class="underline underline-offset-8 text-white cursor-pointer hover:bg-white "> Freepik</a></p>
            <div class="flex justify-start ">
            <p class="bg-[#f49ea8] hover:bg-[#259bca]  text-white px-10 py-3 font-bold text-lg rounded-full tracking-widest">LEARN MORE</p>
          </div>
          </div>
          <div class=" flex self-end lg:pl-[110px] md:pl-96 sm:pl-72 pl-20">
            <img class="lg:min-h-[300px] min-h-[262px] lg:mt-0 mt-36 md:ml-0 dm:ml-0 sm:pl-0 pl-0 xl:max-w-6/12 lg:max-w-6/12  md:max-w-5/12 sm:max-w-5/12 max-w-full object-[44% 50%] object-cover" src="https://images02.nicepage.com/c461c07a441a5d220e8feb1a/6baa3038983251ae8c7607a8/yhjcg.jpg"/>
          </div>
        </div>
      </div>
    </section>






    <!-- third section -->
      <section class="lg:min-h-[850px]  md:min-h-[700px] min-h-[1020px] bg-[#f9c9ce] ">
        <div class=" md:pt-16 lg:p-8 lg:pt-16 xl-10 pt-20 sm:p-8 p-8 relative " > 
          <div class="w-52 color-white absolute mt-[-1rem] xl:left-20 left-0">
            <svg  xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" xml:space="preserve" class="u-svg-content fill-white" viewBox="0 0 160 160" x="0px" y="0px" id="svg-0a30"><path d="M114.3,152.3l38-38C144.4,130.9,130.9,144.4,114.3,152.3z M117.1,9.1l-108,108c0.8,1.6,1.7,3.2,2.7,4.8l110-110
            C120.3,10.9,118.7,10,117.1,9.1z M97.5,2L2,97.5c0.4,2,1,4,1.5,5.9l99.9-99.9C101.5,2.9,99.5,2.4,97.5,2z M80,160c2,0,4-0.1,5.9-0.2
          l73.9-73.9c0.1-2,0.2-3.9,0.2-5.9c0-0.6,0-1.2,0-1.9L78.1,160C78.8,160,79.4,160,80,160z M34.9,146.1c1.5,1,3,2,4.6,2.9L149,39.5
          c-0.9-1.6-1.9-3.1-2.9-4.6L34.9,146.1z M132.7,19.8L19.8,132.7c1.2,1.3,2.3,2.6,3.6,3.9L136.6,23.4C135.3,22.2,134,21,132.7,19.8z
          M59.6,157.4l97.8-97.8c-0.5-1.9-1.1-3.8-1.7-5.7L53.9,155.6C55.8,156.3,57.7,156.9,59.6,157.4z M7.6,45.9L45.9,7.6
          C29.1,15.5,15.5,29.1,7.6,45.9z M80,0c-2.6,0-5.1,0.1-7.6,0.4l-72,72C0.1,74.9,0,77.4,0,80c0,0.1,0,0.2,0,0.2L80.2,0
          C80.2,0,80.1,0,80,0z"></path></svg>
        </div>
        <div class="absolute bottom-[-58px] xl:right-16 right-0  ">
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" xml:space="preserve" class="u-svg-content lg:w-64 md:w-52 w-40 fill-[#2530c9]" viewBox="0 0 160 160" x="0px" y="0px" id="svg-afd0" style="enable-background:new 0 0 160 160;"><path d="M80,30c27.6,0,50,22.4,50,50s-22.4,50-50,50s-50-22.4-50-50S52.4,30,80,30 M80,0C35.8,0,0,35.8,0,80s35.8,80,80,80
	            s80-35.8,80-80S124.2,0,80,0L80,0z"></path></svg>
        </div>
          <div class="relative bg-cover grid md:grid-cols-2 bg-white xl:mx-28 lg:mx-12 md:mx-10 mt-10 ">
            <div class=" bg-center bg-cover lg:min-h-[530px] sm:min-h-[400px]  min-h-[350px] " style="background-image: url('https://images02.nicepage.com/c461c07a441a5d220e8feb1a/b636ec18c64a51a29345d6f8/n.jpg?version=');">
            </div>
          <div>
            <div class="bg-white h-full flex align-left justify-center items-center lg:p-24 lg:p-12 p-6">
              <div>
                <h2  class="font-semibold font-[Oswald , sans-serif] sm:text-5xl text-2xl my-5 text-[#2530c9]">Creative Thinking</h2>
                <p class="my-5">Sample text. Lorem ipsum dolor sit amet, consectetur adipiscing elit nullam nunc justo sagittis suscipit ultrices.</p>
                <p>Images from <a href="# " class="text-decoration-none text-black"> Freepik</a></p>
                <div>
                  <button class="rounded-full px-14 text-xl py-3 bg-[#f49ea8] hover:bg-[#259bca]  font-bold my-5 text-white ">Learn More</button>
                </div>
                </div>
              </div>
            </div>
          </div>
          <div class="absolute sm:right-64 right-32 mt-10">
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" xml:space="preserve" class="u-svg-content w-48 fill-[#f49ea8]" viewBox="0 0 160 100" x="0px" y="0px" id="svg-696e"><path d="M133,27.2c-13.9,9.9-25.8,9.9-39.8,0c-9.1-6.4-16.8-6.4-25.9,0c-13.8,9.8-25.1,9.8-38.9,0c-9.2-6.5-15.4-6.5-24.6,0L0,22.4
	c11.2-8,20.6-8.3,32.2,0c11,7.8,19,8.7,31.3,0c11.6-8.3,22.4-7.9,33.5,0c11.4,8.2,20.3,8.5,32.2,0c11.6-8.3,19.2-8.3,30.8,0
	l-3.8,4.8C146.9,20.6,142.3,20.6,133,27.2z M133,11c-13.9,9.9-25.8,9.9-39.8,0c-9.1-6.4-16.8-6.4-25.9,0c-13.8,9.8-25.1,9.8-38.9,0
	C19.2,4.5,13,4.5,3.8,11L0,6.2c11.2-8,20.6-8.3,32.2,0c11,7.8,19,8.7,31.3,0c11.6-8.3,22.4-7.9,33.5,0c11.4,8.2,20.3,8.5,32.2,0
	c11.6-8.3,19.2-8.3,30.8,0l-3.8,4.8C146.9,4.4,142.3,4.4,133,11z M32.2,38.8c11,7.8,19,8.7,31.3,0c11.6-8.3,22.4-7.9,33.5,0
	c11.4,8.2,20.3,8.5,32.2,0c11.6-8.3,19.2-8.3,30.8,0l-3.8,4.8c-9.3-6.6-13.9-6.6-23.3,0c-13.9,9.9-25.8,9.9-39.8,0
	c-9.1-6.4-16.8-6.4-25.9,0c-13.8,9.8-25.1,9.8-38.9,0c-9.2-6.5-15.4-6.5-24.6,0L0,38.8C11.2,30.8,20.6,30.5,32.2,38.8z M133,76.2
	c-13.9,9.9-25.8,9.9-39.8,0c-9.1-6.4-16.8-6.4-25.9,0c-13.8,9.8-25.1,9.8-38.9,0c-9.2-6.5-15.4-6.5-24.6,0L0,71.4
	c11.2-8,20.6-8.3,32.2,0c11,7.8,19,8.7,31.3,0c11.6-8.3,22.4-7.9,33.5,0c11.4,8.2,20.3,8.5,32.2,0c11.6-8.3,19.2-8.3,30.8,0
	l-3.8,4.8C146.9,69.6,142.3,69.6,133,76.2z M133,60c-13.9,9.9-25.8,9.9-39.8,0c-9.1-6.4-16.8-6.4-25.9,0c-13.8,9.8-25.1,9.8-38.9,0
	c-9.2-6.5-15.4-6.5-24.6,0L0,55.2c11.2-8,20.6-8.3,32.2,0c11,7.8,19,8.7,31.3,0c11.6-8.3,22.4-7.9,33.5,0c11.4,8.2,20.3,8.5,32.2,0
	c11.6-8.3,19.2-8.3,30.8,0l-3.8,4.8C146.9,53.4,142.3,53.4,133,60z M32.2,87.8c11,7.8,19,8.7,31.3,0c11.6-8.3,22.4-7.9,33.5,0
	c11.4,8.2,20.3,8.5,32.2,0c11.6-8.3,19.2-8.3,30.8,0l-3.8,4.8c-9.3-6.6-13.9-6.6-23.3,0c-13.9,9.9-25.8,9.9-39.8,0
	           c-9.1-6.4-16.8-6.4-25.9,0c-13.8,9.8-25.1,9.8-38.9,0c-9.2-6.5-15.4-6.5-24.6,0L0,87.8C11.2,79.8,20.6,79.5,32.2,87.8z"></path></svg>
          </div>
        </div>
      </section>

    <!-- Fourth section -->
      <section id="project" class="">
        <div class="sm:grid grid-cols-1 xl:grid-cols-3 lg:grid-cols-3 md:grid-cols-3 sm:grid-cols-1 md:pb-0 pb-10">
          <div class="w-full col-span-2 py-10 font-sans">
            <div class="lg:pl-16 xl:pl-24 sm:pl-24 pl-5">
              <p class="text-xl font-normal text-black my-4">WHAT WE DO</p>
              <h1 class="text-[#2530c9] sm:text-5xl font-semibold my-4 text-4xl">About Us & Our Work</h1>
              <p class="text-[1.115rem] text-black xl:pr-64 sm:pr-10 md:pr-0 lg:pr-20 pr-10">Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
            </div>
            <div class=" grid grid-cols-1 pt-8" >
              <div>
              <div class=" text-3xl text-black lg:pl-16 xl:pl-24 sm:pl-24 pl-5" >
                <i class="fi fi-rs-angle-right"></i>
              </div>
             </div>
          </div>
        </div>

        <div class="flex relative flex-col justify-center gap-12 px-4 md:mt-32 md:pb-16 sm:pb-48 leading-tight text-white md:justify-self-center min-w-[250px]  md:pb-0 sm:pb-40 pb-4 md:px-0 sm:px-40 px-10">
          <div class="bg-[#fc1aad]  md:min-w-[250px] px-8 py-14 max-w-[350px] lg:max-w-[250px]">
            <P class="font-semibold text-lg tracking-wide">CLIENTS</P>
            <p class="font-bold text-8xl">8k</p>
          </div>
          <div class="bg-[#5ca4fb] md:min-w-[250px] text-white xl:min-w-[26rem] max-w-[350px] lg:min-w-[20rem] lg:min-h-[380px] xl:min-h-[380px] min-h-[236px]  pt-20 px-4 leading-tight lg:mt-32  md:absolute md:mt-32 xl:mt-32 lg:ml-[-23rem] xl:ml-[-30rem] md:ml-[-16rem] sm:ml[-10rem]  xl:pt-20 lg:pt-20 md:pt-20  pt-14" >
                <p class="font-bold xl:text-2xl px-4 tracking-wide md:text-lg sm:text-lg lg:text-2xl text-lg">AWARDS</p>
                <P class="font-bold lg:text-[9rem] xl:text-[9rem]  text-8xl">10k</P>       
            </div>
          <div class="bg-[#2530c9] md:min-w-[250px] lg:min-w-[20rem] max-w-[350px] xl:min-w-[26rem] xl:min-h-[380px] lg:min-h-[380px] sm:min-h-[236px] md:min-h-[236px] min-h-[236px] px-5 py-10 xl:pt-20 lg:pt-20 md:pt-20 sm:pt-14 pt-14">
            <P class="font-bold xl:text-2xl lg:text-2xl px-4 tracking-wide  md:text-lg sm:text-lg lg:text-2xl text-lg">CASES</P>
            <p class="font-bold lg:text-[9rem] xl:text-[9rem]  md:text-8xl sm:text-8xl text-8xl">15k</p>
          </div>
        </div>
        <div class=" md:self-center sm:absolute absolute xl:mt-32 lg:mt-32 md:mt-40  mt-0 sm:grid grid-cols-3  relative self-end">
          <p class="w-full text-black text-[1.125rem]  xl:pl-24 lg:pr-10 md:pl-24 sm:mt-32 sm:px-0 px-10" >Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
        </div>
      </div>     
      </section>


      <!-- Fifth Section -->
      <section class="bg-[#f9c9ce] relative text-center lg:min-h-[180px] xl:min-h-[180px] md:min-h-[180px] min-h-[280px] ">
        <div class="grid xl:grid-cols-2 lg:grid-cols-2 md:grid-cols-2 sm:grid-cols-1 grid-cols-1 pt-16 ">
          <div>
            <p class="text-[#2530c9] text-4xl font-semibold font-sans ">Do you need a consultation?</p>
          </div>
          <div class="flex justify-center  lg:pt-0 xl:pt-0 md:pt-0 sm:pb-10 pt-6">
            <p class="bg-[#2530c9] hover:bg-[#259bca] text-white flex absolute px-8 py-4 font-bold text-lg rounded-full tracking-widest ">LEARN MORE</p>
          </div>
        </div>
      </section>
 
      
      <!-- Sixth Section -->
      <section id="portfolio">
        <div class="">
          <div class="grid xl:grid-cols-3 xl:p-10 xl:gap-8  xl:mx-32 xl:my-16  lg:grid-cols-3 lg:p-2 lg:gap-4 lg:grid-cols-3 lg:mx-6 lg:my-16 md:p-2 md:gap-4  md:mx-4 md:my-8 md:grid-cols-3 gap-8 sm:p-2 sm:gap-4  sm:mx-4 sm:my-8 sm:grid-cols-2 grid-cols-1 my-10 mx-10">
            <div class="min-h-[350px] w-full bg-cover bg-right" style="background-image: url('https://images03.nicepage.com/a1389d7bc73adea1e1c1fb7e/ef7cc744e0f654df97590493/pexelsphoto.jpg');">
            </div>
            <div class="min-h-[350px] bg-cover bg-right " style="background-image: url('https://images03.nicepage.com/a1389d7bc73adea1e1c1fb7e/211b2b64ede85f66968f0782/pexelsphoto1020325.jpeg');">
            </div>
            <div class="min-h-[350px] bg-cover bg-right " style="background-image: url('https://images03.nicepage.com/a1389d7bc73adea1e1c1fb7e/6926bdee16a654e1bc41c8d8/pexelsphoto1037992.jpeg');">
            </div>
            <div class="min-h-[350px] bg-cover bg-right " style="background-image: url('https://images03.nicepage.com/a1389d7bc73adea1e1c1fb7e/f2f1a9dbdce35041ae38ed4e/pexelsphoto2457317.jpg');">
            </div>
            <div class="flex items-center justify-center self-center min-h-[350px] ">
              <p class=" text-[#2530c9] font-semibold text-5xl text-center ">Our Portfolio</p>
            </div>
            <div class="min-h-[350px] bg-cover bg-right " style="background-image: url('https://images03.nicepage.com/a1389d7bc73adea1e1c1fb7e/8d42ce89fed45fad8b9b278b/pexelsphoto1858409.jpeg');">
            </div>
            <div class="min-h-[350px] bg-cover bg-right " style="background-image: url('https://images03.nicepage.com/a1389d7bc73adea1e1c1fb7e/58bfc16b75a3581ab21f9df5/pexelsphoto403571.jpeg');">
            </div>
            <div class="min-h-[350px] bg-cover bg-right " style="background-image: url('https://images03.nicepage.com/a1389d7bc73adea1e1c1fb7e/105150add4bf5f158431ad53/pexelsphoto821652.jpeg');">
            </div>
            <div class="min-h-[350px] bg-cover bg-right " style="background-image: url('https://images03.nicepage.com/a1389d7bc73adea1e1c1fb7e/e71c47348b255d6783ccdc6a/pexelsphoto2333293.jpeg');">
            </div>
          </div>
        </div>
      </section>


      <!-- Seventh Section -->
      <section>
        <div class="grid lg:grid-cols-3 sm:mb-1 lg:mb-0 xl:mb-0 sm:grid-cols-1 grid-cols-1">
          <div class="w-full bg-[#2530c9] col-span-2 flex justify-center">
            <div  class="text-white py-12  flow text-center">
              <div class="pt-12 pb-16 ">
                <p class="text-2xl font-normal tracking-widest">EXCEPTEUR SINT OCCAECAT CUPIDATAT </p>
                <p class="font-semibold sm:text-6xl text-5xl ">Development</p>
              </div>
              <div class="pt-12 pb-16">
                <p class="text-2xl font-normal tracking-widest">DUIS AUTE IRURE DOLOR</p>
                <p class="font-semibold sm:text-6xl text-5xl">Leadership</p>
              </div>
              <div class="pt-12 pb-10">
                <p class="text-2xl font-normal tracking-widest">EXCEPTEUR SINT OCCAECAT CUPIDATAT</p>
                <p class="font-semibold sm:text-6xl text-5xl">Leadership</p>
              </div>
            </div>
          </div>
          <div class="md:p-12 sm:p-2 lg:text-start text-center sm:pt-0 pt-8 ">
            <div class="pb-8 sm:">
              <p class="text-[#fc1aaf] text-3xl font-semibold">Address</p>
              <p class="text-black xl:pr-40 lg:pr-20 pt-4 md:pr-10  md:text-base sm:text-lg sm:pr-10 sm:px-0 px-12">1600 Amphitheatre Parkway, Mountain View, CA 94043</p>
            </div>
            <div class="pb-8">
              <p class="text-[#fc1aaf] text-3xl font-semibold">Phone</p>
              <a href="tel:998-249-9155" class="text-black lg:pr-32 pt-4 text-base sm:pr-0  hover:bg-[#ffffff00]">+91 998 249 9155</a>
            </div>
            <div class="pb-8">
              <p class="text-[#fc1aaf] text-3xl font-semibold">Email</p>
              <a href="mailto:lokendrasingh07773@email.com" class="pt-4 font-bold text-[#2530c9] underline underline-offset-4 text-lg hover:bg-[#ffffff00]">@example.com</a>
            </div>

            <div class="sm:grid sm:justify-items-center lg:justify-items-start md:justify-items-center xl:justify-items-start grid justify-items-center mb-10">
              <div class="min-h-[1px] w-3/6 bg-[#5ca4fb] mt-16"></div>
              <div class="pt-4 px-4">
                <a target="blank" class="hover:bg-white" href="https://www.facebook.com/lokendra.singhmertiya.589?mibextid=2JQ9oc"><i class="fi fi-brands-facebook text-[#3B5998] text-3xl pr-4"></i></a>                
                <a target="blank" class="hover:bg-white" href="https://www.instagram.com/lokendra_banna7773"><i class="fi fi-brands-instagram  text-[#C536A4] text-3xl pr-4"></i></a>
                <a target="blank" class="hover:bg-white" href="https://www.twitter.com/LokendraBanna19"><i class="fi fi-brands-twitter text-[#03a9f4] text-3xl pr-4"></i></a>
                <a target="blank" class="hover:bg-white" href="https://wa.me/9982499155"><i class="fi fi-brands-whatsapp  text-[#39ae41] text-3xl pr-4"></i></a>
              </div>
            </div>
          </div>
        </div><i class=""></i>
      </section>


      <!-- Eight Section -->
      <section class="bg-[#2530c9]">
        <div class="grid grid-cols-1 lg:grid-cols-3 xl:grid-cols-3 md:grid-cols-3 sm:grid-cols-3 py-16 text-white xl:mx-48 lg:justify-items-center xl:justify-items-center md:justify-items-center  sm:mx-5 lg:mx-10 mx-10">
          <div class="sm:pb-0 md:pb-0 lg:pb-0 pb-10">
            <p class="font-semibold text-lg ">Headline</p>
            <p class="pt-2 xl:pr-16 lg:pr-5 md:pr-5 sm:pr-5 pr-0">Sample text. Click to select the text box. Click again or double click to start editing the text.</p>
          </div>
          <div class="sm:pb-0 md:pb-0 lg:pb-0 pb-10">
            <p class="font-semibold text-lg">Headline</p>
            <p class="pt-2">Sample footer text.</p>
          </div>
          <div>
            <p class="font-semibold text-lg">Headline</p>
            <p  class="pt-2">Sample footer text.</p>
          </div>
        </div>
      </section>

      <section class="bg-black min-h-[75px] flex justify-center items-center">
        <div >
          <a target="blank" href="https://www.microprixs.com" class="text-white  hover:bg-[#ffffff00] "> @copyright Microprixs Solution Pvt. Ltd</a>          
        </div>
      </section>
</template>

<style>
.interiorDesign{
  background-image: url('./../assets/images/aser-min.jpg');

}
 .font-sans.bg-\[\#2530c9\].lg\:absolute.md\:relative.sm\:p-8.p-8.sm\:py-10.align-bottom.shadow-2xl.shadow-indigo-500\/50.sm\:block.sm\:p-0.sm\:py-0{
  animation: MyDiv;
  animation-duration: 1s;
  animation-iteration-count: 1;
  animation-timing-function: ease-in;
  animation-direction: normal;
 }
 @keyframes MyDiv {
  0%   {left: 0px; }
  100%  {left: 300px; }
}

.font-sans.bg-\[\#3e427e\].lg\:absolute.sm\:p-8.p-8.sm\:py-10.align-bottom.shadow-2xl.shadow-indigo-500\/50.sm\:block{
  animation: MyDiv1;
  animation-duration: 1s;
  animation-iteration-count: 1;
  animation-timing-function: ease-in;
  animation-direction: normal;
}

@keyframes MyDiv1 {
  0%   {right: 0px; }
  100%  {right: 300px; }
}

.flex.relative.flex-col.justify-center.gap-12.px-4.md\:mt-32.md\:pb-16.sm\:pb-48.leading-tight.text-white.md\:justify-self-center.min-w-\[250px\].md\:pb-0.sm\:pb-40.pb-4.md\:px-0.sm\:px-40.px-10{
  animation: MyDiv2;
  animation-duration: 2s;
  animation-iteration-count: 1;
  animation-timing-function: ease-in;
  animation-direction: normal;
}
@keyframes MyDiv2 {
  0%   {right: -340px; }
  100%  {right: 0px; }
}

.bg-white.md\:w-full.text-black.py-16.px-8.shadow-2xl{
  animation: MyDiv_a;
  animation-duration: 2s;
  animation-iteration-count: 1;
  animation-timing-function: ease-in;
  animation-direction: normal;
}
@keyframes MyDiv_a {
  0%   {right: 0px; }
  100%  {right: 340px; }
}
</style>


<!--   <div class="w-48 color-white">
          <svg  xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" xml:space="preserve" class="u-svg-content fill-white" viewBox="0 0 160 160" x="0px" y="0px" id="svg-0a30"><path d="M114.3,152.3l38-38C144.4,130.9,130.9,144.4,114.3,152.3z M117.1,9.1l-108,108c0.8,1.6,1.7,3.2,2.7,4.8l110-110
	C120.3,10.9,118.7,10,117.1,9.1z M97.5,2L2,97.5c0.4,2,1,4,1.5,5.9l99.9-99.9C101.5,2.9,99.5,2.4,97.5,2z M80,160c2,0,4-0.1,5.9-0.2
	l73.9-73.9c0.1-2,0.2-3.9,0.2-5.9c0-0.6,0-1.2,0-1.9L78.1,160C78.8,160,79.4,160,80,160z M34.9,146.1c1.5,1,3,2,4.6,2.9L149,39.5
	c-0.9-1.6-1.9-3.1-2.9-4.6L34.9,146.1z M132.7,19.8L19.8,132.7c1.2,1.3,2.3,2.6,3.6,3.9L136.6,23.4C135.3,22.2,134,21,132.7,19.8z
	 M59.6,157.4l97.8-97.8c-0.5-1.9-1.1-3.8-1.7-5.7L53.9,155.6C55.8,156.3,57.7,156.9,59.6,157.4z M7.6,45.9L45.9,7.6
	C29.1,15.5,15.5,29.1,7.6,45.9z M80,0c-2.6,0-5.1,0.1-7.6,0.4l-72,72C0.1,74.9,0,77.4,0,80c0,0.1,0,0.2,0,0.2L80.2,0
	C80.2,0,80.1,0,80,0z"></path></svg>
        </div> -->