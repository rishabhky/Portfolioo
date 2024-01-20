<script>
  import { onMount } from 'svelte';

  let showNav = false;

  function toggleNav() {
    showNav = !showNav;
  }

  
</script>

<head>
  <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" />
</head>

<div class="background-container">
  <div class="static blob-container w-max h-fit mx-fit flex-1 flex-col">
    <div class="absolute  w-full h-full flex flex-col justify-start items-center">

      <div class="absolute z-20 flex flex-row backdrop-blur-md {showNav==true?'flex flex-row justify-between rounded-xl':'flex flex-row rounded-xl justify-between'} items-center md:justify-between bg-gray-400 bg-opacity-10 md:m-5 w-full h-fit p-2 md:w-4/5 md:rounded-full md:flex md:flex-row ">
        <a class="font-normal w-1/3 text-gray-700 opacity-70 font-sans font-semibold text-3xl flex justify-center md:text-center select-none">Rishabh</a>

        <nav class="navbar">
          <ul class="flex flex-auto items-center justify-evenly ">
            <div class="flex items-center justify-between ">
              <li><a class="font-semibold  hover:text-gray-900 text-lg px-2 font-sans text-gray-600">About</a></li>
              <li><a class="font-semibold hover:text-gray-900 text-lg px-2 font-sans text-gray-600">Projects</a></li>
              <li><a class="font-semibold hover:text-gray-900 text-lg px-2 font-sans text-gray-600">Skills</a></li>
              <li><a class="font-semibold hover:text-gray-900 text-lg px-2 font-sans text-gray-600">Contact</a></li>
            </div>
            <li class="bg-slate-200 text-gray-700 hover:text-black bg-opacity-50 flex justify-center rounded-full text-base h-10 w-40 font-semibold hover:bg-opacity-5 "><a href="/">Contact Me</a></li>
          </ul>
        </nav>
        <span class="mr-5">
          <svg xmlns="http://www.w3.org/2000/svg" on:click={toggleNav} class="icon" height="16" width="14" viewBox="0 0 448 512"><path fill="#ffffff" d="M0 96C0 78.3 14.3 64 32 64H416c17.7 0 32 14.3 32 32s-14.3 32-32 32H32C14.3 128 0 113.7 0 96zM0 256c0-17.7 14.3-32 32-32H416c17.7 0 32 14.3 32 32s-14.3 32-32 32H32c-17.7 0-32-14.3-32-32zM448 416c0 17.7-14.3 32-32 32H32c-17.7 0-32-14.3-32-32s14.3-32 32-32H416c17.7 0 32 14.3 32 32z" /></svg>
        </span>
      </div>

      <div class="static  flex flex-col justify-center md:mt-32 items-center md:hidden md:bg-transparent {showNav==true?'bg-gray-400 bg-opacity-5 w-full h-30% p-10':''}">
        {#if showNav}
        <div class="burger">
          <a class="font-medium hover:text-gray-200 hover:bg-slate-200 hover:bg-opacity-10 hover:p-3 hover:px-10 hover:rounded-full text-lg font-sans text-gray-400 py-2">About</a>
          <a class="font-medium hover:text-gray-200 hover:bg-slate-200 hover:bg-opacity-10 hover:p-3 hover:px-10 hover:rounded-full mb-5 text-lg font-sans text-gray-400 py-2 ">Projects</a>
          <a class="font-medium hover:text-gray-200 hover:bg-slate-200 hover:bg-opacity-10 hover:p-3 hover:px-10 hover:rounded-full text-lg font-sans text-gray-400 py-2">Skill</a>
          <li class="bg-slate-200 bg-opacity-50 flex justify-center items-center rounded-full text-base h-10 w-40 font-semibold hover:bg-opacity-5"><a href="/">Contact Me</a></li>
        </div>
        {/if}
      </div>

      <body class="z-10 h-screen mx-auto flex-col flex-wrap md:items-start  md:justify-center items-center overflow-y-scroll">
        <div class="static flex flex-col h-screen items-start flex-wrap md:items-center justify-around md:flex-row md:justify-evenly">
          <div class="flex flex-wrap flex-col md:items-center justify-center w-full md:w-1/2 h-fit items-start p-20">
            <span class="text-gray-700 font-semibold text-center flex flex-nowrap font-sans  text-5xl pb-2">👋 Hello, I'm Rishabh !</span>
            <span class="text-gray-700 font-medium font-sans text-center text-xl flex flex-wrap flex-colstext-xl  ml-10">Mobile App Developer and a passionate Front-End Web Developer. With a creative mind and a love for turning ideas into seamless digital experiences, I'm here to showcase my journey in the world of web and mobile development. </span>
          </div>
          <!-- <div class="img  items-center justify-center w-1/3 hidden md:flex">
            <script src="https://unpkg.com/@lottiefiles/lottie-player@latest/dist/lottie-player.js"></script><lottie-player src="https://lottie.host/82786b8c-03c1-4547-9578-322df809f9c9/deDVDdmTIm.json" background="##FFFFFF" speed="1" style="width: 600px; height: 600px" loop  autoplay direction="1" mode="normal"></lottie-player>
          </div> -->
        </div>
        <div class=" flex flex-col justify-center items-center">
          <h1 class="text-gray-600 text-5xl font-semibold ">Projects</h1>
          <ul class="z-10 w-3/4  pt-10 flex flex-col items-center justify-between">
            <li>
              <div class='h-fit w-fit bg-gray-500 bg-opacity-20 shadow-md backdrop-blur-lg rounded-2xl flex flex-col md:flex-row md:justify-around items-center md:mb-10'>
                <img src="src\assets\logo seventify-3.png" alt="Seventify" class="static h-fit w-fit  md:h-1/4 md:w-1/4 rounded-[50px] p-10">
                <span class=" p-5 text-justify md:py-5 md:pr-5  flex-1 flex-col item-center justify-center">
                  <h1 class="text-gray-600 text-4xl font-semibold  flex items-center justify-center md:justify-start">Seventify</h1>
                  <h2 class="text-gray-600 text-2xl font-semibold flex items-center justify-center text-center md:text-left md:justify-start pb-2">Attendance Tracking and Task Management App 📅</h2>
                  <p class="text-gray-600 text-xl font-medium  flex items-center justify-center  text-center md:text-left">Seventify is a comprehensive mobile application designed to streamline attendance tracking and task management for students of all levels. Developed using the Flutter framework and integrated with Firebase for real-time data management, Seventify offers a user-friendly and efficient solution to enhance the academic and organizational experience.</p>
                  <h2 class="text-gray-600 text-2xl font-semibold flex items-center justify-center text-center md:text-left md:justify-start pt-2">Available on Play Store : </h2>
                  <h2 class="text-gray-600 text-xl font-medium flex items-center justify-center text-center md:text-left md:justify-start ">Seventify is now available for download on the Google Play Store, providing easy access for Android users.  </h2>
                </span>
              </div>
            </li>
            <li>
              <div class='h-fit w-fit bg-gray-500 bg-opacity-20 shadow-md backdrop-blur-lg rounded-2xl flex flex-col md:flex-row md:justify-around items-center md:mb-10'>
                <img src="src\assets\Home Harbor.png" alt="HomeHarbor" class="static h-fit w-fit  md:h-1/4 md:w-1/4 rounded-[50px] p-10">
                <span class=" p-5 text-justify md:py-5 md:pr-5  flex-1 flex-col item-center justify-center">
                  <h1 class="text-gray-600 text-4xl font-semibold  flex items-center justify-center md:justify-start">Home Harbor</h1>
                  <h2 class="text-gray-600 text-2xl font-semibold flex items-center justify-center text-center md:text-left md:justify-start pb-2">Society Management App </h2>
                  <p class="text-gray-600 text-xl font-medium  flex items-center justify-center  text-center md:text-left">Home Harbor is a robust mobile application developed to streamline the management of residential societies. Built using the Flutter framework and seamlessly integrated with Firebase, this app provides an all-in-one solution for society members to handle maintenance payments, stay informed through a notice board, and engage in constructive communication via a dedicated chat feature.</p>
                  <span class="flex flex-row justify-center items-center md:p-5 p-2">
                    <a href="https://github.com/rishabhky/society_app"><img  src="src\assets\git.png" alt="github" class="h-10 mr-5 rounded-xl"></a>
                    <a href=" https://www.linkedin.com/posts/rishabh-yadav-625559275_flutterdevelopment-firebase-appdevelopment-activity-7121526623585140736-UzGZ?utm_source=share&utm_medium=member_desktop"><img src="src\assets\link.svg" alt="linkdln" class="h-10 rounded-xl"></a>
                  </span>
                </span>
              </div>
            </li>
            <li>
              <div class='h-fit fit bg-gray-500 bg-opacity-0'>
                <div class='h-fit w-fit bg-gray-500 bg-opacity-20 shadow-md backdrop-blur-lg rounded-2xl flex flex-col md:flex-row md:justify-around items-center md:mb-10'>
                  <img src="src\assets\seeding.png" alt="HomeHarbor" class="static h-fit w-fit  md:h-1/4 md:w-1/4 rounded-[50px] p-10">
                  <span class=" p-5 text-justify md:py-5 md:pr-5  flex-1 flex-col item-center justify-center">
                    <h1 class="text-gray-600 text-4xl font-semibold  flex items-center justify-center md:justify-start">Agrishaala</h1>
                    <h2 class="text-gray-600 text-2xl font-semibold flex items-center justify-center text-center md:text-left md:justify-start pb-2">Society Management App </h2>
                    <p class="text-gray-600 text-xl font-medium  flex items-center justify-center  text-center md:text-left"> Agrishaala that was developed during the Tech Solistice Hackathon! Agrishaala is a revolutionary solution that empowers farmers by detecting plant diseases, suggesting suitable crops based on soil type, and providing an interactive platform for farmers to share knowledge and support each other. 🚀🌾  </p>
                    <span class="flex flex-row justify-center items-center md:p-5 p-2">
                      <a href="https://github.com/vedantRaikar/plantdisease"><img  src="src\assets\git.png" alt="github" class="h-10 mr-5 rounded-xl"></a>
                      <a href=" https://www.linkedin.com/feed/update/urn:li:activity:7085146659248115712?utm_source=share&utm_medium=member_desktop"><img src="src\assets\link.svg" alt="linkdln" class="h-10 rounded-xl"></a>
                    </span>
                  </span>
                </div>
              </div>
            </li>
          </ul>
        </div>
      </body>

    </div>
  </div>
  <div class=" h-scren w-screen flex items-center justify-center ">
    <div class="absolute top-1/4 left-3/4 w-72 h-72 bg-cyan-400 rounded-full mix-blend-multiply filter blur-xl opacity-60 animate-blob animation-delay-2000"></div>
    <div class="absolute bottom-16 left-1/4 w-72 h-72 bg-lime-200 rounded-full mix-blend-multiply filter blur-xl opacity-60 animate-blob"></div>
    <div class="absolute top-1/2 left-1/2 w-72 h-72 bg-violet-400 rounded-full mix-blend-multiply filter blur-xl opacity-60 animate-blob animation-delay-2000"></div>
    <div class="absolute bottom-60 left-20 w-72 h-72 bg-pink-300 rounded-full mix-blend-multiply filter blur-xl opacity-60 animate-blob animation-delay-4000"></div>
  </div>

</div>
