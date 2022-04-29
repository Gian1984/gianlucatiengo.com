<template>
  <div>
    <main>
      <div class="relative pt-16 pb-32 flex content-center items-center justify-center" style="min-height: 75vh;">
        <div class="absolute inset-0 bg-gray-600">
          <iframe width="100%" height="100%" frameborder="0" marginheight="0" marginwidth="0" title="map" scrolling="no" src='https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d80598.44841121738!2d4.305377849792255!3d50.855211410206046!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47c3a4ed73c76867%3A0xc18b3a66787302a7!2sBruxelles%2C%20Belgique!5e0!3m2!1sfr!2sit!4v1650206261181!5m2!1sfr!2sit' style="filter: grayscale(1) contrast(1.2) opacity(0.4);"></iframe>
        </div>
        <div class="pt-10 bg-gray-900 sm:pt-16 lg:pt-8 lg:pb-14 lg:overflow-hidden">
          <div class="mx-auto max-w-7xl lg:px-8">
            <div class="lg:grid lg:grid-cols-2 lg:gap-8">
              <div class="mx-auto max-w-md px-4 sm:max-w-2xl sm:px-6 sm:text-center lg:px-0 lg:text-left lg:flex lg:items-center">
                <div class="lg:py-24">
                  <h1 class="mt-4 text-4xl tracking-tight font-extrabold text-white sm:mt-5 sm:text-6xl lg:mt-6 xl:text-6xl">
                    <transition
                        appear
                        @before-enter="beforeEnter"
                        @enter="enter"
                    >
                      <span class="block text-pink-700">Gianluca Tiengo</span>
                    </transition>
                    <transition
                        appear
                        @before-enter="beforeEnter"
                        @enter="enter"
                    >
                      <span class="pb-3 block bg-clip-text text-transparent bg-gradient-to-r from-teal-400 sm:pb-5"> Web Developer</span>
                    </transition>
                  </h1>
                  <p class="text-base text-black text-gray-300 sm:text-xl lg:text-lg xl:text-xl">
                    I'm a web developer from Turin, Italy and currently living in Brussels. I enjoy building everything from small business to rich interactive apps. If you are a business seeking a web presence or an employer looking to hire, you can get in touch with me <a href="mailto:gl.tiengo@gmail.com" class="text-teal-500">here</a>.
                  </p>
                </div>
              </div>
              <div class="mt-12 -mb-16 sm:-mb-48 lg:m-0 lg:relative">
                <div class="mx-auto max-w-md px-4 sm:max-w-2xl sm:px-6 lg:max-w-none lg:px-0">
                  <!-- Illustration taken from Lucid Illustrations: https://lucid.pixsellz.io/ -->
                  <transition
                      appear
                      @before-enter="beforeSlide"
                      @enter="slide"
                  >
                    <img class="w-full lg:absolute lg:inset-y-0 lg:left-0 lg:h-full lg:w-auto lg:max-w-none" src="img/Illustration.svg" alt="" />
                  </transition>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div
            class="top-auto bottom-0 left-0 right-0 w-full absolute pointer-events-none overflow-hidden"
            style="height: 70px;"
        >
          <svg
              class="absolute bottom-0 overflow-hidden"
              xmlns="http://www.w3.org/2000/svg"
              preserveAspectRatio="none"
              version="1.1"
              viewBox="0 0 2560 100"
              x="0"
              y="0"
          >
            <polygon
                class="text-gray-300 fill-current"
                points="2560 0 2560 100 0 100"
            ></polygon>
          </svg>
        </div>
      </div>
      <section class="pb-20 bg-gray-300 -mt-24">
        <div class="container mx-auto">
          <div class="flex flex-wrap">
            <div class="lg:pt-12 pt-6 w-full md:w-4/12 px-4 text-center">
              <div class="relative flex flex-col min-w-0 break-words bg-white w-full mb-8 shadow-lg rounded-lg">
                <div class="px-4 py-5 flex-auto">
                  <div class="text-white p-3 text-center inline-flex items-center justify-center mb-5 w-40 h-40">
                    <img src="img/vitrine.png" alt="Brochure_Websites">
                  </div>
                  <h6 class="text-xl font-semibold">Brochure Websites</h6>
                  <p class="mt-2 mb-4 text-sm font-light leading-relaxed mt-4 mb-4 text-gray-700">
                    I design and develop responsive brochure websites to showcase your products and services in alignment with your brand essence, your target audience and your preferences. My websites follow the latest design trends to ensure they’re up to date for years to come.
                  </p>
                </div>
              </div>
            </div>
            <div class="w-full md:w-4/12 px-4 text-center">
              <div class="relative flex flex-col min-w-0 break-words bg-white w-full mb-8 shadow-lg rounded-lg">
                <div class="px-4 py-5 flex-auto">
                  <div class="text-white p-3 text-center inline-flex items-center justify-center w-40 h-40 mb-5 ">
                    <img src="img/e-commerce.svg" alt="E-commerce_Websites">
                  </div>
                  <h6 class="text-xl font-semibold">E-commerce Websites</h6>
                  <p class="mt-2 mb-4 text-sm font-light leading-relaxed mt-4 mb-4 text-gray-700">
                    In addition to designing a beautiful, trendy and modern-looking website that fits with your brand, i will also take care of all technical aspects of the e-commerce side to ensure that everything works without issues. I can set up smooth payment systems, integrations and subscriptions.
                  </p>
                </div>
              </div>
            </div>
            <div class="pt-6 w-full md:w-4/12 px-4 text-center">
              <div class="relative flex flex-col min-w-0 break-words bg-white w-full mb-8 shadow-lg rounded-lg">
                <div class="px-4 py-5 flex-auto">
                  <div class="text-white p-3 text-center inline-flex items-center justify-center w-40 h-40 mb-5">
                    <img src="img/coder.png" alt="Web_Application">
                  </div>
                  <h6 class="text-xl font-semibold">Web Application</h6>
                  <p class="mt-2 mb-4 text-sm font-light leading-relaxed mt-4 mb-4 text-gray-700">
                    I deliver web-based applications that help organizations to keep pace with constantly changing business needs. Such applications boast quick and easy access from anywhere on the Internet, ensure lower hardware and software costs, allow faster time to market, and provide flexible integration with other systems.
                  </p>
                </div>
              </div>
            </div>
          </div>
          <div class="flex flex-wrap items-center mt-32">
            <div class="w-full md:w-5/12 px-4 mr-auto ml-auto">
              <div class="text-gray-600 p-3 text-center inline-flex items-center justify-center w-16 h-16 mb-6 shadow-lg rounded-full bg-gray-100">
                <AcademicCapIcon class="h-10 w-10 text-pink-500"></AcademicCapIcon>
              </div>
              <h3 class="text-3xl mb-2 font-semibold leading-normal">
                Skills & Experience
              </h3>
              <p class="text-base sm:text-lg font-light leading-relaxed mt-4 mb-4 text-gray-700">
                I'm a web developer from Turin, Italy and currently living in Brussels. I enjoy building everything from small business to rich interactive apps. If you are a business seeking a web presence or an employer looking to hire, you can get in touch with me <a href="mailto:gl.tiengo@gmail.com" class="text-teal-500">here</a>.<br><br>
                I create successful responsive website that are fast, easy to use, and build with the best practices. The main area of expertise is full-stack development HTMl, CSS, JS, PHP, building small and medium web apps, animations. I have also experience with popular open-source CMS like Wordpress.<br><br>
                As developer I understand the importance to share knowledge. If only one person knows how to do something, that prevents others from developing and hinders progress. When you manage knowledge and give people a platform to share and access it, you’re opening the door to a whole host of benefits!
              </p>
              <a href="https://letudev.com/" class="font-bold text-gray-800 mt-8 hover:text-teal-500">Check my starter kit resources!</a
              >
            </div>
            <div class="w-full md:w-4/12 px-4 mr-auto ml-auto py-10">
              <div class="relative flex flex-col min-w-0 break-words bg-white w-full mb-6 shadow-lg rounded-lg bg-pink-600">
                <img
                    alt="..."
                    src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?ixlib=rb-1.2.1&amp;ixid=eyJhcHBfaWQiOjEyMDd9&amp;auto=format&amp;fit=crop&amp;w=1051&amp;q=80"
                    class="w-full align-middle rounded-t-lg"
                />
                <blockquote class="relative p-8 mb-4">
                  <svg
                      preserveAspectRatio="none"
                      xmlns="http://www.w3.org/2000/svg"
                      viewBox="0 0 583 95"
                      class="absolute left-0 w-full block"
                      style="height: 95px; top: -94px;"
                  >
                    <polygon
                        points="-30,95 583,95 583,65"
                        class="text-pink-600 fill-current"
                    ></polygon>
                  </svg>
                  <h4 class="text-xl font-bold text-white">
                    Ambition & Integrity
                  </h4>
                  <p class="text-md font-light mt-2 text-white">
                    I approach every challenge with energy and vigour. I come up with innovative solutions and I'm not afraid to think big.
                    I care about my work, my clients and my people. I treat everyone with honesty and respect and expect to be treated in the same way.
                  </p>
                </blockquote>
              </div>
            </div>
          </div>
        </div>
      </section>
      <section class="relative py-20">
        <div
            class="bottom-auto top-0 left-0 right-0 w-full absolute pointer-events-none overflow-hidden -mt-20"
            style="height: 80px;"
        >
          <svg
              class="absolute bottom-0 overflow-hidden"
              xmlns="http://www.w3.org/2000/svg"
              preserveAspectRatio="none"
              version="1.1"
              viewBox="0 0 2560 100"
              x="0"
              y="0"
          >
            <polygon
                class="text-white fill-current"
                points="2560 0 2560 100 0 100"
            ></polygon>
          </svg>
        </div>
        <div class="container mx-auto">
          <!-- Feature section with grid -->
          <div class="relative bg-white py-10 sm:py-10 lg:py-10">
            <div class="mx-auto max-w-md px-4 text-center sm:max-w-3xl sm:px-6 lg:px-8 lg:max-w-7xl">
              <h2 class="text-base font-semibold tracking-wider text-cyan-600 uppercase">Deploy faster</h2>
              <p class="mt-2 text-gray-900 tracking-tight text-3xl mb-2 font-semibold leading-normal">
                Everything you need to deploy your app
              </p>
              <p class="mt-5 mx-auto text-base sm:text-lg font-light leading-relaxed mt-4 mb-4 text-gray-700">
                My approach to website development fuses creativity, technology and data analysis, giving you the platform you.
              </p>
              <div class="mt-12">
                <div class="grid grid-cols-1 gap-8 sm:grid-cols-2 lg:grid-cols-3">
                  <div v-for="feature in features" :key="feature.name" class="pt-6">
                    <div class="flow-root bg-gray-50 rounded-lg px-6 pb-8">
                      <div class="-mt-6">
                        <div>
                        <span class="inline-flex items-center justify-center p-3 bg-gradient-to-r from-teal-500 to-cyan-600 rounded-md shadow-lg">
                          <component :is="feature.icon" class="h-6 w-6 text-white" aria-hidden="true" />
                        </span>
                        </div>
                        <h3 class="mt-8 text-lg font-medium text-gray-900 tracking-tight">{{ feature.name }}</h3>
                        <p class="mt-5 text-sm font-light leading-relaxed mt-4 mb-4 text-gray-700">
                          {{ feature.description }}
                        </p>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>


          <section class="relative block bg-gray-900">
            <div
                class="bottom-auto top-0 left-0 right-0 w-full absolute pointer-events-none overflow-hidden -mt-20"
                style="height: 80px;"
            >
              <svg
                  class="absolute bottom-0 overflow-hidden"
                  xmlns="http://www.w3.org/2000/svg"
                  preserveAspectRatio="none"
                  version="1.1"
                  viewBox="0 0 2560 100"
                  x="0"
                  y="0"
              >
                <polygon
                    class="text-gray-900 fill-current"
                    points="2560 0 2560 100 0 100"
                ></polygon>
              </svg>
            </div>
            <div class="container mx-auto lg:pt-24 lg:pb-24 pt-16">
              <div>
                <div class="relative mb-22 box2">
                  <div class="absolute inset-x-0 bottom-0" />
                  <div class="max-w-7xl mx-auto sm:px-6 lg:px-8">
                    <div class="relative  sm:rounded-2xl sm:overflow-hidden hidden md:block">
                      <div class=" flow-root">
                        <div class="-my-2">
                          <div class="box-content py-2 relative h-80 overflow-x-auto xl:overflow-visible">
                            <div class="absolute min-w-screen-xl px-4 flex space-x-8 sm:px-6 lg:px-8 xl:relative xl:px-0 xl:space-x-0 xl:grid xl:grid-cols-6 xl:gap-x-8">
                              <p v-for="category in galleries" :key="category.name" class="relative w-56 h-56 rounded-lg p-6 flex flex-col overflow-hidden hover:opacity-75 xl:w-auto">
                                <span aria-hidden="true" class="absolute inset-0 zoom">
                                  <img :src="category.imageSrc" alt="category-imgage" class="w-56 h-56 object-center object-cover" />
                                </span>
                                <span aria-hidden="true" class="absolute inset-x-0 bottom-0 h-2/3 bg-gradient-to-t from-gray-800 opacity-50" />
                                <span class="relative mt-auto text-center text-xl font-bold text-white">{{ category.name }}</span>
                              </p>
                            </div>
                          </div>
                        </div>
                      </div>
                    </div>
                    <div class="max-w-7xl mx-auto pb-24 px-4 sm:px-6 lg:px-8 md:hidden">
                      <div class="grid grid-cols-2 gap-8 md:grid-cols-6 lg:grid-cols-5">
                        <div v-for="category in galleries" :key="category.name" class="col-span-1 flex justify-center md:col-span-2 lg:col-span-1">
                          <img class="h-24 object-center object-cover" :src="category.imageSrc" alt="tech we use illustration" />
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </section>




          <!-- Blog section -->
          <div class="relative bg-gray-white py-10 sm:py-10 lg:py-10">
            <div
                class="bottom-auto top-0 left-0 right-0 w-full absolute pointer-events-none overflow-hidden -mt-20"
                style="height: 80px;"
            >
              <svg
                  class="absolute bottom-0 overflow-hidden"
                  xmlns="http://www.w3.org/2000/svg"
                  preserveAspectRatio="none"
                  version="1.1"
                  viewBox="0 0 2560 100"
                  x="0"
                  y="0"
              >
                <polygon
                    class="text-white fill-current"
                    points="2560 0 2560 100 0 100"
                ></polygon>
              </svg>
            </div>
            <div class="relative">
              <div class="text-center mx-auto max-w-md px-4 sm:max-w-3xl sm:px-6 lg:px-8 lg:max-w-7xl">
                <h2 class="text-base font-semibold tracking-wider text-cyan-600 uppercase">At Work</h2>
                <p class="mt-2 text-gray-900 tracking-tight text-3xl mb-2 font-semibold leading-normal">
                  This is how we do it
                </p>
                <p class="mt-5 mx-auto text-base sm:text-lg font-light leading-relaxed mt-4 mb-4 text-gray-700">
                  Depending on the type of project, the basic steps of building a website can vary. Not all websites are the same. Different types of management and planning are required.
                </p>
              </div>
              <div class="mt-12 mx-auto max-w-md px-4 grid gap-8 sm:max-w-lg sm:px-6 lg:px-8 lg:grid-cols-3 lg:max-w-7xl">
                <div v-for="post in blogPosts" :key="post.id" class="flex flex-col rounded-lg shadow-lg overflow-hidden">
                  <div class="flex-shrink-0 bg-white">
                    <img class="h-48 mx-auto object-cover" :src="post.image" alt="" />
                  </div>
                  <div class="flex-1 bg-white p-6 flex flex-col justify-between">
                    <div class="flex-1">
                      <p class="text-sm font-medium text-cyan-600">
                        {{ post.category.name }}
                      </p>
                      <a :href="post.href" class="block mt-2">
                        <p class="text-xl font-semibold text-gray-900">
                          {{ post.title }}
                        </p>
                        <p class="mt-3 text-sm font-light leading-relaxed mt-4 mb-4 text-gray-700">
                          {{ post.preview }}
                        </p>
                      </a>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>

      </section>

      <section>
        <!-- Testimonial section -->
        <div class="bg-gradient-to-r from-teal-500 to-cyan-600 relative mx-auto pt-20 pb-12 px-4 sm:px-6 lg:px-8 lg:py-18">
          <div class="relative lg:flex lg:items-center">
            <div class="hidden lg:block lg:flex-shrink-0">
              <img class="h-24 w-24 rounded-full xl:h-40 xl:w-40" src="img/gian.jpg" alt="gianluca_tiengo" />
            </div>

            <div class="relative lg:ml-10">
              <svg class="absolute top-0 left-0 transform -translate-x-8 -translate-y-24 h-36 w-36 text-indigo-200 opacity-50" stroke="currentColor" fill="none" viewBox="0 0 144 144" aria-hidden="true">
                <path stroke-width="2" d="M41.485 15C17.753 31.753 1 59.208 1 89.455c0 24.664 14.891 39.09 32.109 39.09 16.287 0 28.386-13.03 28.386-28.387 0-15.356-10.703-26.524-24.663-26.524-2.792 0-6.515.465-7.446.93 2.327-15.821 17.218-34.435 32.11-43.742L41.485 15zm80.04 0c-23.268 16.753-40.02 44.208-40.02 74.455 0 24.664 14.891 39.09 32.109 39.09 15.822 0 28.386-13.03 28.386-28.387 0-15.356-11.168-26.524-25.129-26.524-2.792 0-6.049.465-6.98.93 2.327-15.821 16.753-34.435 31.644-43.742L121.525 15z" />
              </svg>
              <blockquote class="relative">
                <div class="text-base sm:text-lg text-white font-light leading-relaxed mt-4 mb-4 sm:max-w-7xl">
                  <p>
                    One of the important skills as a Self-taught developer is to be resourceful, my father taught me this skill when I was still very young, and I didn’t know it would take me far in life.
                    I started with wordpress for fun, and my curiosity led me to my first HTML / CSS site. Working during the day, at night I took courses on SoloLearn and all the online platforms that could satiate my desire to learn.<br><br>
                    I realized then that making websites was what I wanted for myself, and I took the time to attend a bootcamp in programming to get better and learn more.<br>
                    Through this learning journey that continues to this day, I am happy and I continue to apply the same principles to what is finally my job today.<br><br>

                    <span class="text-pink-500 font-bold">Re-source-ful</span>
                    <i>  — Having the ability to find clever ways to overcome difficulties.</i>
                  </p>
                </div>
                <footer class="mt-8">
                  <div class="flex">
                    <div class="flex-shrink-0 lg:hidden">
                      <img class="h-12 w-12 rounded-full" src="img/gian.jpg" alt="gianluca_tiengo" />
                    </div>
                  </div>
                </footer>
              </blockquote>
            </div>
          </div>
        </div>
        <div class="relative bg-indigo-800">
          <div class="absolute inset-0">
            <img class="w-full h-full object-cover" src="img/letyoudev.webp" alt="lettudev" />
          </div>
          <div class="relative max-w-7xl mx-auto py-20 px-4 sm:py-24 sm:px-6 lg:px-8">
            <h1 class="text-3xl  font-extrabold tracking-tight text-white sm:text-4xl lg:text-4xl hidden sm:block">Check it out!</h1>
            <a href="https://letudev.com/" target="_blank" class="mt-4 w-40 flex bg-pink-500 text-white active:bg-pink-600 font-bold uppercase text-xs px-4 py-2 rounded-full shadow hover:shadow-md outline-none focus:outline-none mr-1 mb-1 ease-linear transition-all duration-150 hidden sm:block">
              <p class="flex">
              <span class="flex mt-0.5">New project</span>
              <ArrowCircleRightIcon class="ml-2 h-5 w-5"></ArrowCircleRightIcon>
              </p>
            </a>
          </div>
        </div>
        <div class="mx-auto items-center justify-center text-center p-3" style="background-color: #5e17eb !important;">
          <a href="https://letudev.com/" target="_blank" class="flex w-40 flex bg-pink-500 text-white active:bg-pink-600 font-bold uppercase text-xs px-4 py-2 rounded-full shadow hover:shadow-md outline-none focus:outline-none mr-1 mb-1 ease-linear transition-all duration-150 mx-auto block lg:hidden">
            <p class="flex">
            <span class="flex mt-0.5">New project</span>
            <ArrowCircleRightIcon class="ml-2 h-5 w-5"></ArrowCircleRightIcon>
            </p>
          </a>
        </div>
      </section>

      <section class="pt-20 pb-20">
        <div class="container mx-auto">

          <div class="bg-white">
            <div class="mx-auto py-1 px-4 text-center sm:px-6 lg:px-8 lg:py-16">
              <div class="space-y-8 sm:space-y-12">
                <div class="space-y-5 sm:mx-auto sm:max-w-xl sm:space-y-4 lg:max-w-5xl">
                  <h2 class="text-4xl font-semibold">Want to take a look at what I like to do?</h2>
                  <p class="text-base sm:text-lg leading-relaxed m-4 text-gray-600">Whichever platform you choose, I’ll make sure your new website shows the best of you, attracts and convert new leads, and provides a great user experience.</p>
                </div>
                <ul role="list" class="mx-auto grid grid-cols-2 gap-x-4 gap-y-8 sm:grid-cols-4 md:gap-x-6 lg:gap-x-16 lg:gap-y-12 xl:grid-cols-4">
                  <li v-for="person in people" :key="person.name">
                    <a :href="person.href" class="space-y-4">
                      <img class="mx-auto h-24 w-24 rounded-full shadow-2xl lg:w-32 lg:h-32 p-1" :src="person.imageUrl" alt="" />
                      <div class="space-y-2">
                        <div class="text-xs font-medium lg:text-sm">
                          <h3 class="text-xl font-semibold text-gray-900">{{ person.name }}</h3>
                          <p class="text-pink-600">{{ person.role }}</p>
                        </div>
                      </div>
                    </a>
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </section>
      <section class="pb-20 relative block bg-gray-900">
        <div
            class="bottom-auto top-0 left-0 right-0 w-full absolute pointer-events-none overflow-hidden -mt-20"
            style="height: 80px;"
        >
          <svg
              class="absolute bottom-0 overflow-hidden"
              xmlns="http://www.w3.org/2000/svg"
              preserveAspectRatio="none"
              version="1.1"
              viewBox="0 0 2560 100"
              x="0"
              y="0"
          >
            <polygon
                class="text-gray-900 fill-current"
                points="2560 0 2560 100 0 100"
            ></polygon>
          </svg>
        </div>
        <div class="container mx-auto lg:pt-24 lg:pb-48 pt-16">
          <div class="flex flex-wrap text-center justify-center">
            <div class="w-full lg:w-6/12 px-4">
              <h2 class="text-4xl font-semibold text-white">Are you ready?</h2>
              <p class="text-base sm:text-lg leading-relaxed mt-4 mb-4 text-gray-500">
                As your partner i do my best, but what's more important is how i will try help you move forward.
                Whether it’s to better align on your business challenge, understand the people you need to reach,
                or define the best process to get there, we do it together as one single, cohesive team.
              </p>
            </div>
          </div>
          <div class="flex flex-wrap mt-12 justify-center">
            <div class="w-full lg:w-3/12 px-4 text-center">
              <div class="text-gray-900 p-3 w-12 h-12 shadow-lg rounded-full bg-white inline-flex items-center justify-center">
                <SparklesIcon class="h-5 w-5 "></SparklesIcon>
              </div>
              <h6 class="text-xl mt-5 font-semibold text-white">
                Easy
              </h6>
              <p class="mt-2 mb-4 text-gray-500 text-sm sm:text-base">
                No matter what level of web expertise you have, the whole process of development will be simple and manageable.
              </p>
            </div>
            <div class="w-full lg:w-3/12 px-4 text-center">
              <div class="text-gray-900 p-3 w-12 h-12 shadow-lg rounded-full bg-white inline-flex items-center justify-center">
                <SearchIcon class="h-5 w-5"></SearchIcon>
              </div>
              <h5 class="text-xl mt-5 font-semibold text-white">
                Focus
              </h5>
              <p class="mt-2 mb-4 text-gray-500 text-sm sm:text-base">
                I dont want to lure you with empty promises and hyperbole. Instead, i prefer results.
              </p>
            </div>
            <div class="w-full lg:w-3/12 px-4 text-center">
              <div class="text-gray-900 p-3 w-12 h-12 shadow-lg rounded-full bg-white inline-flex items-center justify-center">
                <FireIcon class="h-5 w-5"></FireIcon>
              </div>
              <h5 class="text-xl mt-5 font-semibold text-white">Commitment</h5>
              <p class="mt-2 mb-4 text-gray-500 text-sm sm:text-base">
                I know how important is the presence on the web for you, and that's why I'm committed every day to ensure the best result.
              </p>
            </div>
          </div>
        </div>
      </section>
      <section class="relative block py-16 lg:pt-0 bg-gray-900">
        <div class="container mx-auto">
          <div class="flex flex-wrap justify-center lg:-mt-64 -mt-48">
            <div class="w-full lg:w-6/12 px-2 py-5">
                <form ref="form" @submit.prevent="sendEmail">
                  <div class="container px-2 py-12 mx-auto flex">
                    <div class="relative flex flex-col min-w-0 break-words w-full mb-6 shadow-lg rounded-lg bg-gray-300 p-6">
                      <h2 class="text-gray-900 text-3xl font-semibold mb-1 font-medium title-font">Get in touch!</h2>
                      <p class="leading-relaxed mb-5 text-gray-600 text-sm sm:text-base">My inbox is always open. Whether you have a question or just want to say hi, I'll try my best to get back to you!</p>
                      <div class="relative mb-4">
                        <label for="name" class="leading-7 text-xs text-gray-600">Name / Company</label>
                        <input v-model="name" type="text" id="name" name="email" class="w-full bg-white rounded border border-gray-300 focus:border-orange-500 focus:ring-2 focus:ring-orange-200 text-sm outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out" required>
                      </div>
                      <div class="relative mb-4">
                        <label for="email" class="leading-7 text-xs text-gray-600">Email</label>
                        <input v-model="email" type="email" id="email" name="email" class="w-full bg-white rounded border border-gray-300 focus:border-orange-500 focus:ring-2 focus:ring-orange-200 text-sm outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out" required>
                      </div>
                      <div class="relative mb-4">
                        <label for="subject" class="leading-7 text-xs text-gray-600">Subject</label>
                        <input v-model="subject" name="subject" id="subject" type="text" class="w-full bg-white rounded border border-gray-300 focus:border-orange-500 focus:ring-2 focus:ring-orange-200 text-sm outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out" required>
                      </div>
                      <div class="relative mb-4">
                        <label for="message" class="leading-7 text-xs text-gray-600">Message</label>
                        <textarea v-model="message" id="message" name="message" class="w-full bg-white rounded border border-gray-300 focus:border-orange-500 focus:ring-2 focus:ring-orange-200 h-32 text-sm outline-none text-gray-700 py-1 px-3 resize-none leading-6 transition-colors duration-200 ease-in-out" required></textarea>
                      </div>
                      <div class="relative mb-4">
                        <label for="chaptcha" class="leading-7 text-xs text-gray-600">CAPTCHA verification: 6 + 6 = ?</label>
                        <input v-model="chaptcha" name="chaptcha" id="chaptcha" type="text" class="w-full bg-white rounded border border-gray-300 focus:border-orange-500 focus:ring-2 focus:ring-orange-200 text-sm outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out" required>
                      </div>
                      <button v-if="chaptcha == 12" type="submit" value="Send" class="mt-4 w-24 flex bg-pink-500 text-white active:bg-pink-600 font-bold uppercase text-xs px-4 py-2 rounded-full shadow hover:shadow-md outline-none focus:outline-none mr-1 mb-1 ease-linear transition-all duration-150">
                        <span class="flex">
                          <span class="flex mt-0.5">Send</span>
                          <ArrowCircleRightIcon class="ml-2 h-5 w-5"></ArrowCircleRightIcon>
                        </span>
                      </button>
                    </div>
                  </div>

                  <div class="mt-3" v-if="confirmation" >
                    <div v-if="alertsOpen" class="rounded-md bg-green-50 p-4">
                      <div class="flex">
                        <div class="flex-shrink-0">
                          <CheckCircleIcon class="h-5 w-5 text-green-400" aria-hidden="true" />
                        </div>
                        <div class="ml-3">
                          <p class="text-sm font-medium text-green-800">
                            {{ confirmation }}
                          </p>
                        </div>
                        <div class="ml-auto pl-3">
                          <div class="-mx-1.5 -my-1.5">
                            <button v-on:click="closeAlert()" type="button" class="inline-flex bg-green-50 rounded-md p-1.5 text-green-500 hover:bg-green-100 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-green-50 focus:ring-green-600">
                              <span class="sr-only">Dismiss</span>
                              <XIcon class="h-5 w-5" aria-hidden="true" />
                            </button>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>

                </form>
            </div>
          </div>
        </div>
      </section>
    </main>
  </div>
</template>
<script>

import {
  XIcon,
  CheckCircleIcon,
  FireIcon,
  SearchIcon,
  SparklesIcon,
  AcademicCapIcon,
  CloudUploadIcon,
  CogIcon,
  PencilAltIcon,
  QrcodeIcon,
  ServerIcon,
  ShieldCheckIcon,
  ArrowCircleRightIcon,
} from "@heroicons/vue/outline";
import gsap from 'gsap'
import emailjs from '@emailjs/browser';

const galleries = [
  {
    name: 'JS',
    imageSrc: require('../assets/logos/js.png'),
  },
  {
    name: 'VueJS',
    imageSrc: require('../assets/logos/vuejs.png'),
  },
  {
    name: 'Php',
    imageSrc: require('../assets/logos/php.png'),
  },
  {
    name: 'Laravel',
    imageSrc: require('../assets/logos/laravel.png')
  },
  {
    name: 'TailwindCss',
    imageSrc: require('../assets/logos/tailwind.png')
  },
  {
    name: 'Wordpress',
    imageSrc: require('../assets/logos/wordpress.png')
  },
]

const people = [
  {
    name: 'Belga Mobility',
    role: 'Luxury car rental service with a private driver',
    imageUrl:
        require('../assets/logos/BELGA-MOBILITY.png'),
    href:'https://belgamobility.com/',
  },
  {
    name: 'Claudio Fava',
    role: 'Architect',
    imageUrl:
        require('../assets/logos/logo_fava_border.png'),
    href: 'https://www.favaclaudio.com/'
  },
  {
    name: 'Pizza Vino',
    role: 'Best pizza in BXL',
    imageUrl:
        require('../assets/logos/pizza-vino-logo.png'),
    href:'https://pizzavino.be/',
  },
  {
    name: 'Let You Dev',
    role: 'Platform for personal growth in programming',
    imageUrl:
        require('../assets/logos/letudev.png'),
    href:'https://letudev.com/',
  },
  // More people...
]

const features = [
  {
    name: 'Push to Deploy',
    description: 'Knowledge of Git & most common provider of Internet hosting for software development and version control.',
    icon: CloudUploadIcon,
  },
  {
    name: 'Style',
    description: 'Knowledge of most common CSS framework, like Bootstrap & Tailwind, to easily implement user-friendly UIs.',
    icon: PencilAltIcon,
  },
  {
    name: 'Performant',
    description: 'Knowledge of VueJS framework, the most versatile & performant way to make blazing fast the Virtual DOM.',
    icon: QrcodeIcon,
  },
  {
    name: 'Advanced Security',
    description: 'Usage of Laravel framework, the recommended PHP framework for robust application security',
    icon: ShieldCheckIcon,
  },
  {
    name: 'Powerful API',
    description:
        'API management, to simplify how you connect with your partners, (the Google Maps API is a popular example).',
    icon: CogIcon,
  },
  {
    name: 'Hosting',
    description: 'Administrate hosting service, manage your email accounts or setup a Wordpress instance.',
    icon: ServerIcon,
  },
]

const blogPosts = [
  {
    id: 1,
    title: 'Roadmap',
    href: '#',
    date: 'Mar 16, 2020',
    datetime: '2020-03-16',
    category: { name: 'Stage 1' },
    image:
        require('../assets/map.png'),
    preview:
        'To define the vision of a product or service, I take the time to listen to you and understand your needs and those of your customers. I write a document with the technical specifications, some mockups, a program and a budget estimate.',
  },
  {
    id: 2,
    title: 'Prototyping',
    href: '#',
    date: 'Mar 10, 2020',
    datetime: '2020-03-10',
    category: { name: 'Stage 2' },
    image:
        require('../assets/prototyping.png'),
    preview:
        'There is no universal and precise formula, because each project can have different characteristics. At the beginning we have to define objectives and potential critical issues, after which we move on to the conception of the product and then to the creation of a prototype.',
  },
  {
    id: 3,
    title: 'Development',
    href: '#',
    date: 'Feb 12, 2020',
    datetime: '2020-02-12',
    category: { name: 'Stage 3' },
    image:
        require('../assets/developer.png'),
    preview:
        'Do you have the vision, feel the pull and all you need is software? I will work with you to develop this new functional and design product that your customers will love to use. And I\'ll help you get started.',
  },
]

export default {
  name: "landing-page",

  components:{
    XIcon,
    CheckCircleIcon,
    FireIcon,
    SearchIcon,
    SparklesIcon,
    CloudUploadIcon,
    CogIcon,
    PencilAltIcon,
    QrcodeIcon,
    ServerIcon,
    ShieldCheckIcon,
    ArrowCircleRightIcon,
    AcademicCapIcon
  },

  data() {
    return {
      alertsOpen: true,
      subject:'',
      name:'',
      email: '',
      message: '',
      confirmation:'',
      chaptcha:'',
    }
  },

  methods: {
    sendEmail() {
      try {
        emailjs.sendForm('service_58mft2p', 'template_dhvckrb', this.$refs.form, 'AmnMprCMW3riak6qR', {
          name: this.name,
          subject: this.subject,
          email: this.email,
          message: this.message
        })
      } catch (error) {
        console.log({error})
      }
      // Reset form field
          this.name = '',
          this.subject = '',
          this.email = '',
          this.message = ''
          this.chaptcha = ''
          this.confirmation = 'Your messase has been sent!'
    },

    closeAlert: function(){
      this.alertsOpen = false;
    },

  },

  setup() {
      const beforeEnter = (el) => {
        el.style.opacity = 0
        el.style.transform = 'translateX(400px)'
      }
      const enter = (el, done) => {
        gsap.to(el, {
          opacity: 1,
          x: 0,
          duration: 1.5,
          onComplete: done,
          delay: el.dataset.index * 0.5
        })
      }

      const beforeSlide = (el) => {
        el.style.opacity = 0
        el.style.transform = 'translateY(400px)'
      }

      const slide = (el, done) => {
        gsap.to(el, {
          opacity: 1,
          y: 0,
          duration: 1.5,
          onComplete: done,
          delay: el.dataset.index * 0.2,
          rotation: 360,
        })
      }

      return {
        galleries,
        people,
        features,
        blogPosts,
        beforeEnter,
        enter,
        slide,
        beforeSlide,
      }
    },

}
</script>
