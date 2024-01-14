<template>

    <body class="bg-gray-100">
    <header>
        <nav class="fixed z-20 w-full bg-cyan-900 backdrop-blur navbar shadow-2xl shadow-gray-600/5 border-gray-100 dark:border-gray-200 peer-checked:navbar-active dark:shadow-none border-b">
            <div class="xl:container m-auto px-6 md:px-12 lg:px-6">
                <div class="flex flex-wrap items-center justify-between gap-6 md:py-3 md:gap-0 lg:py-5">
                    <div class="w-full items-center flex justify-between lg:w-auto">
                        <label for="hbr" class="peer-checked:hamburger block relative z-20 p-6 -mr-6 cursor-pointer lg:hidden">
                            <div aria-hidden="true" class="m-auto h-0.5 w-5 rounded bg-gray-900 dark:bg-gray-300 transition duration-300"></div>
                            <div aria-hidden="true" class="m-auto mt-2 h-0.5 w-5 rounded bg-gray-900 dark:bg-gray-300 transition duration-300"></div>
                        </label>
                    </div>
                    <div class="navmenu hidden w-full flex-wrap justify-end items-center mb-16 space-y-8 p-6 border border-gray-100 rounded-3xl shadow-2xl shadow-gray-300/20 bg-white lg:space-y-0 lg:p-0 lg:m-0 lg:flex md:flex-nowrap lg:bg-transparent lg:w-7/12 lg:shadow-none dark:shadow-none dark:border-gray-700 lg:border-0">
                        <div class="text-gray-600 dark:text-gray-300 lg:pr-4">
                            <ul class="space-y-6 tracking-wide font-medium text-base lg:text-sm lg:flex lg:space-y-0">
                                <li>
                                    <a href="/" class="block md:px-4 transition text-gray-100">
                                        <span>Home</span>
                                    </a>
                                </li>
                                <li>
                                    <a href="/portfolio" class="block md:px-4 transition text-gray-100">
                                        <span>Portfolio</span>
                                    </a>
                                </li>
                                <li>
                                    <a href="/services" class="block md:px-4 transition text-gray-100">
                                        <span>Services</span>
                                    </a>
                                </li>
                            </ul>
                        </div>

                        <div class="w-full space-y-2 border-primary/10 dark:border-gray-700 flex flex-col -ml-1 sm:flex-row lg:space-y-0 md:w-max lg:border-l">
                            <a href="/info" class="relative flex h-9 ml-auto items-center justify-center sm:px-6 before:absolute before:inset-0 before:rounded-full focus:before:bg-sky-600/10 dark:focus:before:bg-sky-400/10 before:transition before:duration-300 hover:before:scale-105 active:duration-75 active:before:scale-95">
                                <span class="relative text-sm font-semibold text-gray-100">Contact Us</span>
                            </a>
                            <a href="/login" class="relative flex h-9 ml-auto items-center justify-center sm:px-6 before:absolute before:inset-0 before:rounded-full before:bg-blue-700 dark:before:bg-blue-500 before:transition before:duration-300 hover:before:scale-105 active:duration-75 active:before:scale-95">
                                <span class="relative text-sm font-semibold text-gray-100">Login</span>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </nav>
    </header>

<div class="bg-gray-100 justify-center pt-8">
  <div class="flex flex-col items-center justify-between pt-0 pb-0 mt-0 mr-auto mb-0 ml-auto max-w-7xl
      xl:px-5 lg:flex-row">
    <div class="flex flex-col items-center w-full pt-5 pr-10 pb-20 pl-10 lg:pt-20 lg:flex-row">
      <div class="w-full bg-cover relative max-w-md lg:max-w-2xl lg:w-7/12">
        <div class="flex flex-col items-center justify-center w-full h-full relative lg:pr-10">
          <img src="https://res.cloudinary.com/macxenon/image/upload/v1631570592/Run_-_Health_qcghbu.png" class="btn-"/>
        </div>
      </div>
      <div class="w-full mt-20 mr-0 mb-0 ml-0 relative z-10 max-w-2xl lg:mt-0 lg:w-5/12">
        <form @submit.prevent="saveContact()">
        <div class="flex flex-col items-start justify-start pt-10 pr-10 pb-10 pl-10 bg-white shadow-2xl rounded-xl
            relative z-10">
          <p class="w-full text-4xl text-cyan-900 font-large text-center leading-snug font-serif">Contact Form</p>
          <p class="w-full font-medium text-center leading-snug mt-2">RE: daniel@digitalpulse.si</p>
          <div class="w-full mt-6 mr-0 mb-0 ml-0 relative space-y-8">
            <div class="relative">
              <p class="bg-white pt-0 pr-2 pb-0 pl-2 -mt-3 mr-0 mb-0 ml-2 font-medium text-cyan-900
                  absolute">Name</p>
              <input placeholder="Your Name" type="text" v-model="message.name" class="border placeholder-gray-400 focus:outline-none
                  focus:border-black w-full pt-4 pr-4 pb-4 pl-4 mt-2 mr-0 mb-0 ml-0 text-base block bg-white
                  border-gray-300 rounded-md"
                  />
            </div>
            <div class="relative">
              <p class="bg-white pt-0 pr-2 pb-0 pl-2 -mt-3 mr-0 mb-0 ml-2 font-medium text-cyan-900 absolute">Email</p>
              <input placeholder="example@domain.com" type="text" v-model="message.mail_address" class="border placeholder-gray-400 focus:outline-none
                  focus:border-black w-full pt-4 pr-4 pb-4 pl-4 mt-2 mr-0 mb-0 ml-0 text-base block bg-white
                  border-gray-300 rounded-md"/>
            </div>
            <div class="relative">
              <p class="bg-white pt-0 pr-2 pb-0 pl-2 -mt-3 mr-0 mb-0 ml-2 font-medium text-cyan-900
                  absolute">Message</p>
                  <textarea id="description" name="description" placeholder="Write your message here..." v-model="message.description" class="border placeholder-gray-400 focus:outline-none
                  focus:border-black w-full pt-4 pr-4 pb-4 pl-4 mt-2 mr-0 mb-0 ml-0 text-base block bg-white
                  border-gray-300 rounded-md" rows="7"></textarea>
            </div>
            <div class="relative">
              <button @click="handleButtonClick" type="submit" class="w-full inline-block pt-4 pr-5 pb-4 pl-5 text-xl font-medium text-center text-white bg-cyan-900
                  rounded-lg transition duration-200 hover:bg-cyan-700 ease">Submit</button>
            </div>
          </div>
          <p v-if="submissionResult === 'success'" class="w-full font-medium text-center leading-snug mt-4 text-green-800">Your inquiry has been received!</p>
        <p v-if="submissionResult === 'error'" class="w-full font-medium text-center leading-snug mt-4 text-red-500">Submit failed. Please check your entries.</p>
        </div>
    </form>
        <svg viewbox="0 0 91 91" class="absolute top-0 left-0 z-0 w-32 h-32 -mt-12 -ml-12 text-yellow-300
            fill-current"><g stroke="none" strokewidth="1" fillrule="evenodd"><g fillrule="nonzero"><g><g><circle
            cx="3.261" cy="3.445" r="2.72"/><circle cx="15.296" cy="3.445" r="2.719"/><circle cx="27.333" cy="3.445"
            r="2.72"/><circle cx="39.369" cy="3.445" r="2.72"/><circle cx="51.405" cy="3.445" r="2.72"/><circle cx="63.441"
            cy="3.445" r="2.72"/><circle cx="75.479" cy="3.445" r="2.72"/><circle cx="87.514" cy="3.445" r="2.719"/></g><g
            transform="translate(0 12)"><circle cx="3.261" cy="3.525" r="2.72"/><circle cx="15.296" cy="3.525"
            r="2.719"/><circle cx="27.333" cy="3.525" r="2.72"/><circle cx="39.369" cy="3.525" r="2.72"/><circle
            cx="51.405" cy="3.525" r="2.72"/><circle cx="63.441" cy="3.525" r="2.72"/><circle cx="75.479" cy="3.525"
            r="2.72"/><circle cx="87.514" cy="3.525" r="2.719"/></g><g transform="translate(0 24)"><circle cx="3.261"
            cy="3.605" r="2.72"/><circle cx="15.296" cy="3.605" r="2.719"/><circle cx="27.333" cy="3.605" r="2.72"/><circle
            cx="39.369" cy="3.605" r="2.72"/><circle cx="51.405" cy="3.605" r="2.72"/><circle cx="63.441" cy="3.605"
            r="2.72"/><circle cx="75.479" cy="3.605" r="2.72"/><circle cx="87.514" cy="3.605" r="2.719"/></g><g
            transform="translate(0 36)"><circle cx="3.261" cy="3.686" r="2.72"/><circle cx="15.296" cy="3.686"
            r="2.719"/><circle cx="27.333" cy="3.686" r="2.72"/><circle cx="39.369" cy="3.686" r="2.72"/><circle
            cx="51.405" cy="3.686" r="2.72"/><circle cx="63.441" cy="3.686" r="2.72"/><circle cx="75.479" cy="3.686"
            r="2.72"/><circle cx="87.514" cy="3.686" r="2.719"/></g><g transform="translate(0 49)"><circle cx="3.261"
            cy="2.767" r="2.72"/><circle cx="15.296" cy="2.767" r="2.719"/><circle cx="27.333" cy="2.767" r="2.72"/><circle
            cx="39.369" cy="2.767" r="2.72"/><circle cx="51.405" cy="2.767" r="2.72"/><circle cx="63.441" cy="2.767"
            r="2.72"/><circle cx="75.479" cy="2.767" r="2.72"/><circle cx="87.514" cy="2.767" r="2.719"/></g><g
            transform="translate(0 61)"><circle cx="3.261" cy="2.846" r="2.72"/><circle cx="15.296" cy="2.846"
            r="2.719"/><circle cx="27.333" cy="2.846" r="2.72"/><circle cx="39.369" cy="2.846" r="2.72"/><circle
            cx="51.405" cy="2.846" r="2.72"/><circle cx="63.441" cy="2.846" r="2.72"/><circle cx="75.479" cy="2.846"
            r="2.72"/><circle cx="87.514" cy="2.846" r="2.719"/></g><g transform="translate(0 73)"><circle cx="3.261"
            cy="2.926" r="2.72"/><circle cx="15.296" cy="2.926" r="2.719"/><circle cx="27.333" cy="2.926" r="2.72"/><circle
            cx="39.369" cy="2.926" r="2.72"/><circle cx="51.405" cy="2.926" r="2.72"/><circle cx="63.441" cy="2.926"
            r="2.72"/><circle cx="75.479" cy="2.926" r="2.72"/><circle cx="87.514" cy="2.926" r="2.719"/></g><g
            transform="translate(0 85)"><circle cx="3.261" cy="3.006" r="2.72"/><circle cx="15.296" cy="3.006"
            r="2.719"/><circle cx="27.333" cy="3.006" r="2.72"/><circle cx="39.369" cy="3.006" r="2.72"/><circle
            cx="51.405" cy="3.006" r="2.72"/><circle cx="63.441" cy="3.006" r="2.72"/><circle cx="75.479" cy="3.006"
            r="2.72"/><circle cx="87.514" cy="3.006" r="2.719"/></g></g></g></g></svg>
        <svg viewbox="0 0 91 91" class="absolute bottom-0 right-0 z-0 w-32 h-32 -mb-12 -mr-12 text-indigo-500
            fill-current"><g stroke="none" strokewidth="1" fillrule="evenodd"><g fillrule="nonzero"><g><g><circle
            cx="3.261" cy="3.445" r="2.72"/><circle cx="15.296" cy="3.445" r="2.719"/><circle cx="27.333" cy="3.445"
            r="2.72"/><circle cx="39.369" cy="3.445" r="2.72"/><circle cx="51.405" cy="3.445" r="2.72"/><circle cx="63.441"
            cy="3.445" r="2.72"/><circle cx="75.479" cy="3.445" r="2.72"/><circle cx="87.514" cy="3.445" r="2.719"/></g><g
            transform="translate(0 12)"><circle cx="3.261" cy="3.525" r="2.72"/><circle cx="15.296" cy="3.525"
            r="2.719"/><circle cx="27.333" cy="3.525" r="2.72"/><circle cx="39.369" cy="3.525" r="2.72"/><circle
            cx="51.405" cy="3.525" r="2.72"/><circle cx="63.441" cy="3.525" r="2.72"/><circle cx="75.479" cy="3.525"
            r="2.72"/><circle cx="87.514" cy="3.525" r="2.719"/></g><g transform="translate(0 24)"><circle cx="3.261"
            cy="3.605" r="2.72"/><circle cx="15.296" cy="3.605" r="2.719"/><circle cx="27.333" cy="3.605" r="2.72"/><circle
            cx="39.369" cy="3.605" r="2.72"/><circle cx="51.405" cy="3.605" r="2.72"/><circle cx="63.441" cy="3.605"
            r="2.72"/><circle cx="75.479" cy="3.605" r="2.72"/><circle cx="87.514" cy="3.605" r="2.719"/></g><g
            transform="translate(0 36)"><circle cx="3.261" cy="3.686" r="2.72"/><circle cx="15.296" cy="3.686"
            r="2.719"/><circle cx="27.333" cy="3.686" r="2.72"/><circle cx="39.369" cy="3.686" r="2.72"/><circle
            cx="51.405" cy="3.686" r="2.72"/><circle cx="63.441" cy="3.686" r="2.72"/><circle cx="75.479" cy="3.686"
            r="2.72"/><circle cx="87.514" cy="3.686" r="2.719"/></g><g transform="translate(0 49)"><circle cx="3.261"
            cy="2.767" r="2.72"/><circle cx="15.296" cy="2.767" r="2.719"/><circle cx="27.333" cy="2.767" r="2.72"/><circle
            cx="39.369" cy="2.767" r="2.72"/><circle cx="51.405" cy="2.767" r="2.72"/><circle cx="63.441" cy="2.767"
            r="2.72"/><circle cx="75.479" cy="2.767" r="2.72"/><circle cx="87.514" cy="2.767" r="2.719"/></g><g
            transform="translate(0 61)"><circle cx="3.261" cy="2.846" r="2.72"/><circle cx="15.296" cy="2.846"
            r="2.719"/><circle cx="27.333" cy="2.846" r="2.72"/><circle cx="39.369" cy="2.846" r="2.72"/><circle
            cx="51.405" cy="2.846" r="2.72"/><circle cx="63.441" cy="2.846" r="2.72"/><circle cx="75.479" cy="2.846"
            r="2.72"/><circle cx="87.514" cy="2.846" r="2.719"/></g><g transform="translate(0 73)"><circle cx="3.261"
            cy="2.926" r="2.72"/><circle cx="15.296" cy="2.926" r="2.719"/><circle cx="27.333" cy="2.926" r="2.72"/><circle
            cx="39.369" cy="2.926" r="2.72"/><circle cx="51.405" cy="2.926" r="2.72"/><circle cx="63.441" cy="2.926"
            r="2.72"/><circle cx="75.479" cy="2.926" r="2.72"/><circle cx="87.514" cy="2.926" r="2.719"/></g><g
            transform="translate(0 85)"><circle cx="3.261" cy="3.006" r="2.72"/><circle cx="15.296" cy="3.006"
            r="2.719"/><circle cx="27.333" cy="3.006" r="2.72"/><circle cx="39.369" cy="3.006" r="2.72"/><circle
            cx="51.405" cy="3.006" r="2.72"/><circle cx="63.441" cy="3.006" r="2.72"/><circle cx="75.479" cy="3.006"
            r="2.72"/><circle cx="87.514" cy="3.006" r="2.719"/></g></g></g></g></svg>
      </div>
    </div>
  </div>
</div>

                <div class="min-h-screen bg-gray-100 flex">
                <div class="container max-w-screen-lg mx-auto">
                <h4 class="text-4xl font-bold text-cyan-900 tracking-widest uppercase text-center">FAQ</h4>
        <p class="text-center text-gray-600 text-sm mt-2">Here are some of the frequently asked questions</p>
        <div class="space-y-12 px-2 xl:px-16 mt-12">
            <div class="mt-4 flex">
                <div>
                    <div class="flex items-center h-16 border-l-4 border-cyan-900">
                        <span class="text-4xl text-cyan-900 px-4">Q.</span>
                    </div>
                    <div class="flex items-center h-16 border-l-4 border-gray-400">
                        <span class="text-4xl text-gray-400 px-4">A.</span>
                    </div>
                </div>
                <div>
                    <div class="flex items-center h-16">
                        <span class="text-lg text-cyan-900 font-bold">Are you a digital agency?</span>
                    </div>
                    <div class="flex items-center py-2">
                        <span class="text-gray-500">No. All services offered on this platform are fulfilled individually meaning you will be working and communicating directly with me, there is no unreliable third-party invovled.</span>

                    </div>
                </div>
            </div>

            <div class="mt-4 flex">
                <div>
                    <div class="flex items-center h-16 border-l-4 border-cyan-900">
                        <span class="text-4xl text-cyan-900 px-4">Q.</span>
                    </div>
                    <div class="flex items-center h-16 border-l-4 border-gray-400">
                        <span class="text-4xl text-gray-400 px-4">A.</span>
                    </div>
                </div>
                <div>
                    <div class="flex items-center h-16">
                        <span class="text-lg text-cyan-900 font-bold">Are you available to work as a freelancer currently?</span>
                    </div>
                    <div class="flex items-center py-2">
                        <span class="text-gray-500">Yes. I'm available to work part-time as a both front and backend developer on various projects.  </span>

                    </div>
                </div>
            </div>

            <div class="mt-4 flex">
                <div>
                    <div class="flex items-center h-16 border-l-4 border-cyan-900">
                        <span class="text-4xl text-cyan-900 px-4">Q.</span>
                    </div>
                    <div class="flex items-center h-16 border-l-4 border-gray-400">
                        <span class="text-4xl text-gray-400 px-4">A.</span>
                    </div>
                </div>
                <div>
                    <div class="flex items-center h-16">
                        <span class="text-lg text-cyan-900 font-bold">Are you able to guarantee on what was agreed upon?</span>
                    </div>
                    <div class="flex items-center py-2">
                        <span class="text-gray-500">Yes. All tasks will be processed via Upwork's platform ensuring both parties meaning you get what you pay for. Learn more about the work process and policies via <a href="" class="text-blue-600">Upwork.</a></span>

                    </div>
                </div>
            </div>

            <div class="mt-4 flex">
                <div>
                    <div class="flex items-center h-16 border-l-4 border-cyan-900">
                        <span class="text-4xl text-cyan-900 px-4">Q.</span>
                    </div>
                    <div class="flex items-center h-16 border-l-4 border-gray-400">
                        <span class="text-4xl text-gray-400 px-4">A.</span>
                    </div>
                </div>
                <div>
                    <div class="flex items-center h-16">
                        <span class="text-lg text-cyan-900 font-bold">What can I expect from your services?</span>
                    </div>
                    <div class="flex items-center py-2">
                        <span class="text-gray-500">Results. I'll assess each inquiry individually which guarantees a personalized approach in accordance with your expectations and all services are ensured with a digital contract with clear <a href="" class="text-blue-600">terms & conditions.</a> </span>

                    </div>
                </div>
            </div>

            <div class="mt-4 flex">
                <div>
                    <div class="flex items-center h-16 border-l-4 border-cyan-900">
                        <span class="text-4xl text-cyan-900 px-4">Q.</span>
                    </div>
                    <div class="flex items-center h-16 border-l-4 border-gray-400">
                        <span class="text-4xl text-gray-400 px-4">A.</span>
                    </div>
                </div>
                <div>
                    <div class="flex items-center h-16">
                        <span class="text-lg text-cyan-900 font-bold">How do we process billing and payments?</span>
                    </div>
                    <div class="flex items-center py-2">
                        <span class="text-gray-500">Individually. Only after we assess the presented task and reach an agreement in terms of the work conditions we will draft a contract via Upwork which acts both as a middle man and the billing processor. </span>

                    </div>
                </div>
            </div>

            <div class="mt-4 flex">
                <div>
                    <div class="flex items-center h-16 border-l-4 border-cyan-900">
                        <span class="text-4xl text-cyan-900 px-4">Q.</span>
                    </div>
                    <div class="flex items-center h-16 border-l-4 border-gray-400">
                        <span class="text-4xl text-gray-400 px-4">A.</span>
                    </div>
                </div>
                <div>
                    <div class="flex items-center h-16">
                        <span class="text-lg text-cyan-900 font-bold">Got any more questions or concerns?</span>
                    </div>
                    <div class="flex items-center py-2">
                        <span class="text-gray-500">Feel free to contact me via the form above or email (daniel@digitalpulse.si).</span>

                    </div>
                </div>
            </div>


                    </div>
                </div>
            </div>


            <footer class="bg-cyan-900 mt-16">
        <div class="container px-6 py-12 mx-auto">
            <div class="grid grid-cols-1 gap-6 sm:grid-cols-2 sm:gap-y-10 lg:grid-cols-4">
                <div class="sm:col-span-2">
                    <h1 class="max-w-lg text-xl  tracking-tight text-gray-800 xl:text-2xl dark:text-white font-serif">Subscribe to the newsletter to get regular educational and promotional content.</h1>

                    <form @submit.prevent="saveData()">
                    <div class="flex flex-col mx-auto mt-6 space-y-3 md:space-y-0 md:flex-row">
                        <input v-model="newsletter.email" id="email" type="text" class="px-4 py-2 text-gray-700 bg-white border rounded-md dark:bg-gray-900 dark:text-gray-300 dark:border-gray-600 focus:border-blue-400 dark:focus:border-blue-300 focus:outline-none focus:ring focus:ring-opacity-40 focus:ring-blue-300" placeholder="Email Address">

                        <button type="submit" class="w-full px-6 py-2.5 text-sm font-medium tracking-wider text-white transition-colors duration-300 transform md:w-auto md:mx-4 focus:outline-none bg-gray-800 rounded-lg hover:bg-gray-700 focus:ring focus:ring-gray-300 focus:ring-opacity-80">
                            Subscribe
                        </button>
                    </div>
                    <p class="text-gray-600 transition-colors duration-300 dark:text-gray-300 dark:hover:text-blue-400 hover:underline hover:text-blue-500 mt-2" v-if="!isValidEmail && email !== ''">
                    Please enter a valid email address.
                    </p>
                </form>
                </div>

                <div>
                    <p class="font-semibold text-gray-800 dark:text-white">Navigation</p>

                    <div class="flex flex-col items-start mt-5 space-y-2">
                        <a href="/" class="text-gray-600 transition-colors duration-300 dark:text-gray-300 dark:hover:text-blue-400 hover:underline hover:text-blue-500">Home</a>
                        <a href="/portfolio" class="text-gray-600 transition-colors duration-300 dark:text-gray-300 dark:hover:text-blue-400 hover:underline hover:text-blue-500">Portfolio</a>
                        <a href="/services" class="text-gray-600 transition-colors duration-300 dark:text-gray-300 dark:hover:text-blue-400 hover:underline hover:text-blue-500">Services</a>
                        <a href="/info" class="text-gray-600 transition-colors duration-300 dark:text-gray-300 dark:hover:text-blue-400 hover:underline hover:text-blue-500">Contact Info</a>
                    </div>
                </div>

                <div>
                    <p class="font-semibold text-gray-800 dark:text-white">Available On</p>

                    <div class="flex flex-col items-start mt-5 space-y-2">
                        <a href="https://www.upwork.com/freelancers/~01e0ea10215a43ee5a" class="text-gray-600 transition-colors duration-300 dark:text-gray-300 dark:hover:text-blue-400 hover:underline hover:text-blue-500">Upwork</a>
                        <a href="https://www.linkedin.com/in/digitalpdaniel/" class="text-gray-600 transition-colors duration-300 dark:text-gray-300 dark:hover:text-blue-400 hover:underline hover:text-blue-500">LinkedIn</a>
                        <a href="https://github.com/daniel-dpsi" class="text-gray-600 transition-colors duration-300 dark:text-gray-300 dark:hover:text-blue-400 hover:underline hover:text-blue-500">GitHub</a>
                    </div>
                </div>
            </div>

            <hr class="my-6 border-gray-200 md:my-8 dark:border-gray-700">


            <div class="flex items-center justify-between">

                <div class="flex -mx-2">
                    <a href="https://github.com/daniel-dpsi" class="mx-2 text-gray-600 transition-colors duration-300 dark:text-gray-300 hover:text-blue-500 dark:hover:text-blue-400" aria-label="Github">
                        <svg class="w-5 h-5 fill-current" viewBox="0 0 24 24" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M12.026 2C7.13295 1.99937 2.96183 5.54799 2.17842 10.3779C1.395 15.2079 4.23061 19.893 8.87302 21.439C9.37302 21.529 9.55202 21.222 9.55202 20.958C9.55202 20.721 9.54402 20.093 9.54102 19.258C6.76602 19.858 6.18002 17.92 6.18002 17.92C5.99733 17.317 5.60459 16.7993 5.07302 16.461C4.17302 15.842 5.14202 15.856 5.14202 15.856C5.78269 15.9438 6.34657 16.3235 6.66902 16.884C6.94195 17.3803 7.40177 17.747 7.94632 17.9026C8.49087 18.0583 9.07503 17.99 9.56902 17.713C9.61544 17.207 9.84055 16.7341 10.204 16.379C7.99002 16.128 5.66202 15.272 5.66202 11.449C5.64973 10.4602 6.01691 9.5043 6.68802 8.778C6.38437 7.91731 6.42013 6.97325 6.78802 6.138C6.78802 6.138 7.62502 5.869 9.53002 7.159C11.1639 6.71101 12.8882 6.71101 14.522 7.159C16.428 5.868 17.264 6.138 17.264 6.138C17.6336 6.97286 17.6694 7.91757 17.364 8.778C18.0376 9.50423 18.4045 10.4626 18.388 11.453C18.388 15.286 16.058 16.128 13.836 16.375C14.3153 16.8651 14.5612 17.5373 14.511 18.221C14.511 19.555 14.499 20.631 14.499 20.958C14.499 21.225 14.677 21.535 15.186 21.437C19.8265 19.8884 22.6591 15.203 21.874 10.3743C21.089 5.54565 16.9181 1.99888 12.026 2Z">
                            </path>
                        </svg>
                    </a>
                </div>
            </div>
        </div>
    </footer>

  </body>


</template>

<script>
//import MainLayout from '@/Layouts/MainLayout.vue';
export default {
    data() {
        return {
            buttonClicked: false,
            btnResponse: "Button has been clicked!",
            submissionResult: null,
            'newsletter':{
                'email': ''
            },
            'message':{
                'name': '',
                'mail_address': '',
                'description': ''
            }
        };
    },
    computed: {
    isValidEmail() {
      // Basic email validation using a regular expression
      const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
      return emailRegex.test(this.newsletter.email);
    },
  },
    methods: {
        saveData() {
            if (this.isValidEmail) {axios.post('/newsletter/submit', this.newsletter).then(
                response => {
                    console.log(response);
                }
            ). catch(error => {
                console.log('Submit failed.');
                this.$router.push('/login');
            })} else {
        // Handle invalid email case (display error, prevent form submission, etc.)
        console.error('Invalid email. Please correct the email address.');
      }

            //console.log("test hello", this.newsletter);
        },
        saveContact() {
            axios.post('/message/submit', this.message).then(
                response => {
                    console.log(response);
                    this.submissionResult = 'success';
                }
            ). catch(error => {
                console.log("error");
                this.submissionResult = 'error';
            })
        },
        handleButtonClick() {
      // Set the buttonClicked to true when the button is clicked
      this.buttonClicked = true;
      setTimeout(() => {
        this.buttonClicked = false;
      }, 3000);
    }
    }
};

</script>

<style>

</style>
