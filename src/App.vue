<template>
  <div class="banner-1">
    <!-- NavBar -->
    <nav
      class="container px-6 mx-auto md:flex md:justify-between md:items-center"
    >
      <div class="flex items-center justify-between">
        <div class="relative w-16 h-16">
          <img
            class="rounded-full border border-gray-100 shadow-sm"
            src="../src/assets/diongwapa.jpg"
            alt="user image"
          />
        </div>
        <!-- Mobile menu button -->
        <div @click="showMenu = !showMenu" class="flex md:hidden">
          <button
            type="button"
            class="text-gray-800 hover:text-gray-400 focus:outline-none focus:text-gray-400"
          >
            <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
              <path
                fill-rule="evenodd"
                d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"
              ></path>
            </svg>
          </button>
        </div>
      </div>
      <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
      <ul
        :class="showMenu ? 'flex' : 'hidden'"
        class="flex-col items-end mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0"
      >
        <li class="menu-button"><a href="#">Home</a></li>
        <li class="menu-button"><a href="#work" v-smooth-scroll>Works</a></li>
        <li class="menu-button"><a href="#about" v-smooth-scroll>About</a></li>
      </ul>
    </nav>
    <!-- End Navbar -->

    <div class="flex items-center">
      <div class="w-11/12 space-y-5 md:space-y-10">
        <h3
          class="hello-button text-gray-700 w-fit md:py-3 md:px-5 py-1 px-2 rounded-lg 3xl:text-3xl 2xl:text-xl lg:text-xl md:text-md text-sm font-semibold font-work_sans"
        >
          👋 Hola,
        </h3>
        <h1
          class="3xl:text-8xl 2xl:text-7xl xl:text-6xl lg:text-4xl md:text-3xl sm:text-3xl text-xl font-Eczar font-bold leading-tight text-gray-700"
        >
          It's
          <a
            href="https://www.facebook.com/diOncelin"
            target="_blank"
            class="text-black hover:underline"
          >
            Dioncelin Sumalinog</a
          >🙇‍♀️<br />Front End Developer
        </h1>
 
      </div>

      <div class="w-8/12 flex justify-end">
        <img
          class="3xl:h-[800px] 2xl:h-[650px] xl:h-[550px] lg:h-[550px] md:h-[450px] sm:h-[350px]"
          src="./assets/profile-female.png"
          alt="user image"
        />
      </div>
    </div>
  </div>

  <div class="banner-2 space-y-10 pb-20" id="work">
    <h3 class="heading3 my-5">My Recent Work</h3>
    <div class="card">
      <div class="space-y-5 py-8 px-8 md:py-16 md:px-20 md:w-1/2">
        <h4 class="project-title item">CPC Safety Central</h4>
        <p class="font-work_sans pr-12">
          CPC Safety Central System is a comprehensive platform designed to ensure the safety and well-being of students, staff, and visitors. This system integrates various components and technologies to monitor, manage, and respond to safety incidents effectively within the school premises.
At its core, the Safety Central System includes features such as surveillance cameras strategically placed throughout the campus to monitor entrances, hallways, and other critical areas in real-time. Access control systems are also implemented to regulate entry and exit points, ensuring that only authorized individuals can access certain areas of the school.
        </p>
      </div>
      <div class="card-image bg-green-100">
        <img
          class="object-cover w-full h-72 md:h-96"
          src="./assets/project1.png"
        />
      </div>
    </div>

    <div class="card">
      <div class="space-y-5 py-8 px-8 md:py-16 md:px-20 md:w-1/2">
        <h4 class="project-title item">Spotify API</h4>
        <p class="font-work_sans pr-12">
          The Spotify API system is a comprehensive platform that allows developers to integrate Spotify's vast music catalog and features into their own applications and services. By leveraging the API, developers can access functionalities such as searching for tracks, albums, and artists, retrieving user playlists, managing user libraries, and playing music directly within their applications. The API provides endpoints for both retrieving data from Spotify's extensive music database and controlling music playback.
        </p>
      </div>
      <div class="card-image">
        <img
          class="object-cover w-full h-48 md:h-96"
          src="./assets/project2.png"
        />
      </div>
    </div>
  </div>


        <div class="absolute inset-y-0 left-0 lg:flex lg:items-center">
          <button
            class="mt-24 lg:mt-0 -ml-6 h-12 w-12 rounded-full bg-white p-3 shadow-lg"
          >
            <svg
              class="h-full w-full text-indigo-900"
              fill="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                d="M5.41 11H21a1 1 0 0 1 0 2H5.41l5.3 5.3a1 1 0 0 1-1.42 1.4l-7-7a1 1 0 0 1 0-1.4l7-7a1 1 0 0 1 1.42 1.4L5.4 11z"
              />
            </svg>
          </button>
        </div>
        <div class="absolute inset-y-0 right-0 lg:flex lg:items-center">
          <button
            class="mt-24 lg:mt-0 -mr-6 h-12 w-12 rounded-full bg-white p-3 shadow-lg"
          >
            <svg
              class="h-full w-full text-indigo-900"
              fill="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                d="M18.59 13H3a1 1 0 0 1 0-2h15.59l-5.3-5.3a1 1 0 1 1 1.42-1.4l7 7a1 1 0 0 1 0 1.4l-7 7a1 1 0 0 1-1.42-1.4l5.3-5.3z"
              />
            </svg>
          </button>
        </div>

  <div class="banner-2 md:flex items-center md:justify-evenly" id="about">
    <img
      class="md:h-[500px] h-[400px]"
      src="./assets/about-female.png"
      alt="user image"
    />
    <div class="space-y-5 py-8 px-8 md:py-16 md:px-20 md:w-1/2">
      <h4 class="project-title item">About Me</h4>
      <p class="font-work_sans">
        I am Dioncelin Sumalinog, Philippines. I am a BSIT student in Cordova Public College.
        <br />
        Welcome to the portfolio of a skilled frontend programmer! Here, you'll find a showcase of meticulously crafted digital experiences that blend creativity with functionality to bring visions to life on the web. As a frontend programmer, I specialize in transforming design concepts into responsive and user-friendly interfaces that captivate and engage audiences.
      </p>
    </div>
  </div>

  <div class="banner-1 flex h-full items-center">
    <div class="w-7/12 p-12">
      <h2 class="text-gray-700 md:text-6xl text-2xl font-Eczar mb-5 font-bold">
        Let’s work together and make everything super cute and super useful.
      </h2>
      <a class="underline text-2xl text-blue-600 font-work_sans"
        >dioncelinsumalinog2001@gmail.com</a
      >
    </div>
    <div class="contact-links">
            <div class="contact-link">
              <a href="https://www.instagram.com/dddddd_yonnnn/"><img src="../src/assets/instagram-icon.png" alt="Instagram Logo" class="contact-logo"></a>
            </div>
            <div class="contact-link">
              <a href="mailto:dioncelin2001@gmail.com"><img src="../src/assets/gmail-icon.png" alt="Gmail Logo" class="contact-logo"></a>
            </div>
            <div class="contact-link">
              <a href="https://www.facebook.com/diOncelin"><img src="../src/assets/facebook.png" alt="Facebook Logo" class="contact-logo"></a>
            </div>
          </div>
  </div>
</template>
<script>
  export default {
    data() {
      return {
        showMenu: false,
      }
    },
  }
</script>
<style scoped>
.contact-links {
  display: flex;
  justify-content: center;
}

.contact-link {
  margin: 0 1rem;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.contact-logo {
  width: 50px;
  height: 50px;
  margin-bottom: 0.5rem;
}

</style>
