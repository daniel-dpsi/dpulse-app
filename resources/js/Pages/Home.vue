<template>


    <body class="bg-white">
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
                                    <a href="#" class="block md:px-4 transition text-gray-100">
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

    <div class="bg-white relative pt-20 pb-20 lg:pt-44">
        <div class="relative xl:container m-auto px-6 md:px-12 lg:px-6">
            <h1 class="sm:mx-auto sm:w-10/12 md:w-2/3 font-black text-cyan-900 text-4xl text-center sm:text-5xl md:text-6xl lg:w-auto lg:text-left xl:text-7xl">Realize your next project with<br class="lg:block hidden"> <span class="relative text-cyan-900 bg-clip-text bg-gradient-to-r from-cyan-600 to-indigo-600">DigitalPulse Solutions</span>.</h1>
            <div class="lg:flex">
                <div class="relative mt-8 md:mt-16 space-y-8 sm:w-10/12 md:w-2/3 lg:ml-0 sm:mx-auto text-center lg:text-left lg:mr-auto lg:w-7/12">
                    <p class="sm:text-lg text-black lg:w-11/12">
                        Our solutions take SMEs to the next level by implementing dynamic and efficient digital solutions. Modern cutting-edge web applications, freelance work, automatization, cloud intergrations, server administration, trainings, consultations and more.
                    </p>
                    <span class="block font-semibold text-gray-700">Experience seamless realization of your ideas.</span>
                    <div class="grid grid-cols-3 space-x-4 md:space-x-6 md:flex md:justify-center lg:justify-start">
                        <a aria-label="add to slack" href="https://github.com/daniel-dpsi" class="p-4 border bg-transparent border-gray-300 rounded-full duration-300 hover:border-cyan-400 hover:shadow-lg hover:shadow-cyan-600/20 dark:hover:border-cyan-300/30">
                            <div class="flex justify-center space-x-4">
                                <img class="w-6 h-6" src="https://img.icons8.com/clouds/128/github.png" alt="apple-mail"  loading="lazy" width="128" height="128">
                                <span class="hidden font-medium md:block text-black">GitHub</span>
                            </div>
                        </a>
                        <a aria-label="add to slack" href="https://www.linkedin.com/in/digitalpdaniel/" class="p-4 border bg-transparent border-gray-300 rounded-full duration-300 hover:border-cyan-400 hover:shadow-lg hover:shadow-cyan-600/20 dark:hover:border-cyan-300/30">
                            <div class="flex justify-center space-x-4">
                                <img class="w-6 h-6" src="https://img.icons8.com/cute-clipart/128/linkedin.png" alt="linkedin logo" loading="lazy" width="128" height="128">
                                <span class="hidden font-medium md:block text-black">LinkedIn</span>
                            </div>
                        </a>
                        <a aria-label="add to slack" href="https://www.upwork.com/freelancers/~01e0ea10215a43ee5a" class="p-4 border bg-transparent border-gray-300 rounded-full duration-300 hover:border-cyan-400 hover:shadow-lg hover:shadow-cyan-600/20 dark:hover:border-cyan-300/30">
                            <div class="flex justify-center space-x-4">
                                <img class="w-6 h-6" src="https://img.icons8.com/external-tal-revivo-green-tal-revivo/128/000000/external-upwork-a-global-freelancing-platform-where-professionals-connect-and-collaborate-remotely-logo-green-tal-revivo.png" alt="upwork logo" loading="lazy" width="128" height="128">
                                <span class="hidden font-medium md:block text-black">Upwork</span>
                            </div>
                        </a>

                    </div>

                    <div class="text-gray-600">
                        <span>For collaboration requests and inquiries: </span>
                        <a href="#" class="font-semibold text-gray-700">daniel@digitalpulse.si</a>
                    </div>

                    <div class="pt-12 pb-12 flex gap-3 justify-between grayscale lg:w-2/3">
                        <!--<img src="https://www.fullstackpython.com/img/logos/vuejs-wide.png" class="h-8 sm:h-10 w-auto lg:h-12" alt="" />
                        <img src="https://techalmas.com/wp-content/uploads/2021/02/Laravel_logo_wordmark_logotype.png" class="h-8 sm:h-10 w-auto lg:h-12" alt="" />
                        <img src="https://assets-global.website-files.com/601064f495f4b4967f921aa9/632b60f8c1aa184a0e5766d9_202209-ms-sql-icon-3x.png" class="h-8 sm:h-10 w-auto lg:h-12" alt="" />-->
                    </div>
                </div>
                <div class="mt-12 md:mt-0 lg:absolute -right-10 lg:w-7/12">
                    <div class="relative w-full">
                        <div aria-hidden="true" class="absolute scale-75 md:scale-110 inset-0 m-auto w-full h-full md:w-96 md:h-96 rounded-full rotate-45 bg-gradient-to-r from-sky-500 to-cyan-300 blur-3xl"></div>
                        <img src="https://tailus.io/sources/blocks/tech-startup/preview/images/globalization-cuate.svg" class="relative w-full" alt="wath illustration" loading="lazy" width="320" height="280">
                    </div>
                </div>
            </div>
        </div>
    </div>

        <footer class="bg-cyan-900 mt-56">
        <div class="container px-6 py-12 mx-auto">
            <div class="grid grid-cols-1 gap-6 sm:grid-cols-2 sm:gap-y-10 lg:grid-cols-4">
                <div class="sm:col-span-2">
                    <h1 class="max-w-lg text-xl  tracking-tight text-gray-800 xl:text-2xl dark:text-white">Subscribe to the newsletter to get regular educational and promotional content.</h1>

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
            'newsletter':{
                'email': ''
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
        }
    }
};

</script>


<style>
.error-message {
  color: rgb(255, 255, 255);
  font-size: 14px;
  margin-top: 5px;
}
</style>
