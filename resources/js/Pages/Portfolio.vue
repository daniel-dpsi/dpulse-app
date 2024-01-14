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



    <div class="pt-32 pb-6 relative text-center xl:container m-auto px-6 md:px-12 lg:px-6">
        <h1 class="sm:mx-auto sm:w-10/12 md:w-2/3 font-black text-cyan-900 text-4xl text-center sm:text-5xl md:text-6xl lg:w-auto lg:text-center xl:text-7xl">Project Overview</h1>
        <h4 class="text-2xl text-black mt-6">Backed By 100% Job Success Rate</h4>
        <p class="text-md text-black mt-1">Empowering robust and dynamic digital envrionments with modern cutting-edge technology.</p>
        </div>

       <!-- <section class="bg-white pt-4 border-b border-t">
                <div class="container mx-auto">
                    <div class="-mx-4 flex flex-wrap">
                    <div class="w-full px-4 md:w-1/2 lg:w-1/3">
                        <div class="relative mx-4 mt-4 overflow-hidden rounded-xl bg-blue-gray-500 bg-clip-border text-white shadow-lg shadow-blue-gray-500/40">
                        <img
                        src="https://apploye.com/blog/content/images/2023/09/alternatives-of-upwork.png"
                        alt="ui/ux review check"
                        />
                        <div class="to-bg-black-10 absolute inset-0 h-full w-full bg-gradient-to-tr from-transparent via-transparent to-black/60"></div>
                        <button
                        class="!absolute top-4 right-4 h-8 max-h-[32px] w-8 max-w-[32px] select-none rounded-full text-center align-middle font-sans text-xs font-medium uppercase text-red-500 transition-all hover:bg-red-500/10 active:bg-red-500/30 disabled:pointer-events-none disabled:opacity-50 disabled:shadow-none"
                        type="button"
                        data-ripple-dark="true"
                        >
                        <span class="absolute top-1/2 left-1/2 -translate-y-1/2 -translate-x-1/2 transform">
                            <svg
                            xmlns="http://www.w3.org/2000/svg"
                            viewBox="0 0 24 24"
                            fill="currentColor"
                            aria-hidden="true"
                            class="h-6 w-6"
                            >
                            <path d="M11.645 20.91l-.007-.003-.022-.012a15.247 15.247 0 01-.383-.218 25.18 25.18 0 01-4.244-3.17C4.688 15.36 2.25 12.174 2.25 8.25 2.25 5.322 4.714 3 7.688 3A5.5 5.5 0 0112 5.052 5.5 5.5 0 0116.313 3c2.973 0 5.437 2.322 5.437 5.25 0 3.925-2.438 7.111-4.739 9.256a25.175 25.175 0 01-4.244 3.17 15.247 15.247 0 01-.383.219l-.022.012-.007.004-.003.001a.752.752 0 01-.704 0l-.003-.001z"></path>
                            </svg>
                        </span>
                        </button>
                    </div>
                    <div class="p-6">
                        <div class="mb-3 flex items-center justify-between">
                        <h5 class="block font-sans text-xl font-medium leading-snug tracking-normal text-blue-gray-900 antialiased">
                            Ralf K. (Quasda GmbH)
                        </h5>
                        <p class="flex items-center gap-1.5 font-sans text-base font-normal leading-relaxed text-blue-gray-900 antialiased">
                            <svg
                            xmlns="http://www.w3.org/2000/svg"
                            viewBox="0 0 24 24"
                            fill="currentColor"
                            aria-hidden="true"
                            class="-mt-0.5 h-5 w-5 text-yellow-700"
                            >
                            <path
                                fill-rule="evenodd"
                                d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
                                clip-rule="evenodd"
                            ></path>
                            </svg>
                            5.0
                        </p>
                        </div>
                        <p class="block font-sans text-base font-light leading-relaxed text-gray-700 antialiased">
                            Great Job, great communication :)
                        </p>

                    </div>
                    <div class="p-6 pt-3">
                        <button
                        class="block w-full select-none rounded-lg bg-indigo-900 py-3.5 px-7 text-center align-middle font-sans text-sm font-bold uppercase text-white shadow-md shadow-blue-500/20 transition-all hover:shadow-lg hover:shadow-indigo-500/40 focus:opacity-[0.85] focus:shadow-none active:opacity-[0.85] active:shadow-none disabled:pointer-events-none disabled:opacity-50 disabled:shadow-none"
                        type="button"
                        data-ripple-light="true"
                        >
                        REVIEW
                        </button>
                    </div>
                    </div>
                    <div class="w-full px-4 md:w-1/2 lg:w-1/3">
                        <div class="relative mx-4 mt-4 overflow-hidden rounded-xl bg-blue-gray-500 bg-clip-border text-white shadow-lg shadow-blue-gray-500/40">
                        <img
                        src="https://apploye.com/blog/content/images/2023/09/alternatives-of-upwork.png"
                        alt="ui/ux review check"
                        />
                        <div class="to-bg-black-10 absolute inset-0 h-full w-full bg-gradient-to-tr from-transparent via-transparent to-black/60"></div>
                        <button
                        class="!absolute top-4 right-4 h-8 max-h-[32px] w-8 max-w-[32px] select-none rounded-full text-center align-middle font-sans text-xs font-medium uppercase text-red-500 transition-all hover:bg-red-500/10 active:bg-red-500/30 disabled:pointer-events-none disabled:opacity-50 disabled:shadow-none"
                        type="button"
                        data-ripple-dark="true"
                        >
                        <span class="absolute top-1/2 left-1/2 -translate-y-1/2 -translate-x-1/2 transform">
                            <svg
                            xmlns="http://www.w3.org/2000/svg"
                            viewBox="0 0 24 24"
                            fill="currentColor"
                            aria-hidden="true"
                            class="h-6 w-6"
                            >
                            <path d="M11.645 20.91l-.007-.003-.022-.012a15.247 15.247 0 01-.383-.218 25.18 25.18 0 01-4.244-3.17C4.688 15.36 2.25 12.174 2.25 8.25 2.25 5.322 4.714 3 7.688 3A5.5 5.5 0 0112 5.052 5.5 5.5 0 0116.313 3c2.973 0 5.437 2.322 5.437 5.25 0 3.925-2.438 7.111-4.739 9.256a25.175 25.175 0 01-4.244 3.17 15.247 15.247 0 01-.383.219l-.022.012-.007.004-.003.001a.752.752 0 01-.704 0l-.003-.001z"></path>
                            </svg>
                        </span>
                        </button>
                    </div>
                    <div class="p-6">
                        <div class="mb-3 flex items-center justify-between">
                        <h5 class="block font-sans text-xl font-medium leading-snug tracking-normal text-blue-gray-900 antialiased">
                            Garret T. (Heidi Computers Ltd)
                        </h5>
                        <p class="flex items-center gap-1.5 font-sans text-base font-normal leading-relaxed text-blue-gray-900 antialiased">
                            <svg
                            xmlns="http://www.w3.org/2000/svg"
                            viewBox="0 0 24 24"
                            fill="currentColor"
                            aria-hidden="true"
                            class="-mt-0.5 h-5 w-5 text-yellow-700"
                            >
                            <path
                                fill-rule="evenodd"
                                d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
                                clip-rule="evenodd"
                            ></path>
                            </svg>
                            4.7
                        </p>
                        </div>
                        <p class="block font-sans text-base font-light leading-relaxed text-gray-700 antialiased">
                            Provided valuable assistance in getting our product working...
                        </p>
                    </div>
                    <div class="p-6 pt-3">
                        <button
                        class="block w-full select-none rounded-lg bg-indigo-900 py-3.5 px-7 text-center align-middle font-sans text-sm font-bold uppercase text-white shadow-md shadow-blue-500/20 transition-all hover:shadow-lg hover:shadow-indigo-500/40 focus:opacity-[0.85] focus:shadow-none active:opacity-[0.85] active:shadow-none disabled:pointer-events-none disabled:opacity-50 disabled:shadow-none"
                        type="button"
                        data-ripple-light="true"
                        >
                        REVIEW
                        </button>
                    </div>
                    </div>
                    <div class="w-full px-4 md:w-1/2 lg:w-1/3">
                        <div class="relative mx-4 mt-4 overflow-hidden rounded-xl bg-blue-gray-500 bg-clip-border text-white shadow-lg shadow-blue-gray-500/40">
                        <img
                        src="https://apploye.com/blog/content/images/2023/09/alternatives-of-upwork.png"
                        alt="ui/ux review check"
                        />
                        <div class="to-bg-black-10 absolute inset-0 h-full w-full bg-gradient-to-tr from-transparent via-transparent to-black/60"></div>
                        <button
                        class="!absolute top-4 right-4 h-8 max-h-[32px] w-8 max-w-[32px] select-none rounded-full text-center align-middle font-sans text-xs font-medium uppercase text-red-500 transition-all hover:bg-red-500/10 active:bg-red-500/30 disabled:pointer-events-none disabled:opacity-50 disabled:shadow-none"
                        type="button"
                        data-ripple-dark="true"
                        >
                        <span class="absolute top-1/2 left-1/2 -translate-y-1/2 -translate-x-1/2 transform">
                            <svg
                            xmlns="http://www.w3.org/2000/svg"
                            viewBox="0 0 24 24"
                            fill="currentColor"
                            aria-hidden="true"
                            class="h-6 w-6"
                            >
                            <path d="M11.645 20.91l-.007-.003-.022-.012a15.247 15.247 0 01-.383-.218 25.18 25.18 0 01-4.244-3.17C4.688 15.36 2.25 12.174 2.25 8.25 2.25 5.322 4.714 3 7.688 3A5.5 5.5 0 0112 5.052 5.5 5.5 0 0116.313 3c2.973 0 5.437 2.322 5.437 5.25 0 3.925-2.438 7.111-4.739 9.256a25.175 25.175 0 01-4.244 3.17 15.247 15.247 0 01-.383.219l-.022.012-.007.004-.003.001a.752.752 0 01-.704 0l-.003-.001z"></path>
                            </svg>
                        </span>
                        </button>
                    </div>
                    <div class="p-6">
                        <div class="mb-3 flex items-center justify-between">
                        <h5 class="block font-sans text-xl font-medium leading-snug tracking-normal text-blue-gray-900 antialiased">
                            Daniel G. (Freelancer)
                        </h5>
                        <p class="flex items-center gap-1.5 font-sans text-base font-normal leading-relaxed text-blue-gray-900 antialiased">
                            <svg
                            xmlns="http://www.w3.org/2000/svg"
                            viewBox="0 0 24 24"
                            fill="currentColor"
                            aria-hidden="true"
                            class="-mt-0.5 h-5 w-5 text-yellow-700"
                            >
                            <path
                                fill-rule="evenodd"
                                d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
                                clip-rule="evenodd"
                            ></path>
                            </svg>
                            5.0
                        </p>
                        </div>
                        <p class="block font-sans text-base font-light leading-relaxed text-gray-700 antialiased">
                            Very helpful and efficient, fixed our server environment...
                        </p>

                    </div>
                    <div class="p-6 pt-3">
                        <button
                        class="block w-full select-none rounded-lg bg-indigo-900 py-3.5 px-7 text-center align-middle font-sans text-sm font-bold uppercase text-white shadow-md shadow-blue-500/20 transition-all hover:shadow-lg hover:shadow-indigo-500/40 focus:opacity-[0.85] focus:shadow-none active:opacity-[0.85] active:shadow-none disabled:pointer-events-none disabled:opacity-50 disabled:shadow-none"
                        type="button"
                        data-ripple-light="true"
                        >
                        REVIEW
                        </button>
                    </div>
                    </div>

                    </div>
                </div>
                </section>-->

        <section class="bg-white pt-10">
                <div class="container mx-auto">
                    <div class="-mx-4 flex flex-wrap">
                        <div class="w-full px-4 md:w-1/2 lg:w-1/3">
                        <div class="mx-auto mb-10 max-w-[370px]">
                        <div class="mb-8 overflow-hidden rounded">
                            <img
                            src="https://cdn.discordapp.com/attachments/923643835073060886/1073206862410944532/image.png?ex=65b248c7&is=659fd3c7&hm=f85591856ce7ba32065aff04b4572d33c2a97fc135d15822c0be8e5f5b8f90d0&"
                            alt="image"
                            class="w-120"
                            />
                        </div>
                        <div>
                            <h3>
                            <a
                                href="javascript:void(0)"
                                class="text-dark hover:text-primary mb-4 inline-block text-xl font-semibold sm:text-2xl lg:text-xl xl:text-2xl"
                            >
                                Digital Learning Platform
                            </a>
                            </h3>
                            <p class="text-body-color text-base">
                                Powering remote education and learning processes for school institutions in form of a web application.
                            </p>
                        </div>
                        </div>
                    </div>
                    <div class="w-full px-4 md:w-1/2 lg:w-1/3">
                        <div class="mx-auto mb-10 max-w-[370px]">
                        <div class="mb-8 overflow-hidden rounded">
                            <img
                            src="https://cdn.discordapp.com/attachments/923643835073060886/1195780533737762827/image.png?ex=65b53c67&is=65a2c767&hm=7170e04c8345246c938473c91a96228b790106889f2ac01e27e53509c5e059c6&"
                            alt="image"
                            class="w-120"
                            />
                        </div>
                        <div>
                            <h3>
                            <a
                                href="javascript:void(0)"
                                class="text-dark hover:text-primary mb-4 inline-block text-xl font-semibold sm:text-2xl lg:text-xl xl:text-2xl"
                            >
                                Third-party API Intergration
                            </a>
                            </h3>
                            <p class="text-body-color text-base">
                                Enables users to make calls directly to the API and display obtained data on their own websites.
                            </p>
                        </div>
                        </div>
                    </div>
                    <div class="w-full px-4 md:w-1/2 lg:w-1/3">
                        <div class="mx-auto mb-10 max-w-[370px]">
                        <div class="mb-8 overflow-hidden rounded">
                            <img
                            src="https://cdn.discordapp.com/attachments/997826356639453245/1033843937724612758/unknown.png?ex=65ad82b2&is=659b0db2&hm=80d6aeddc0dc22766fd50b02b7329eae15b36bd318fdd248e640cc59ead628d4&"
                            alt="image"
                            class="w-120 h-100"
                            />
                        </div>
                        <div>
                            <h3>
                            <a
                                href="javascript:void(0)"
                                class="text-dark hover:text-primary mb-4 inline-block text-xl font-semibold sm:text-2xl lg:text-xl xl:text-2xl"
                            >
                                Endpoint API Development
                            </a>
                            </h3>
                            <p class="text-body-color text-base">
                                Powering an E-Commerce platform that allows for administration and overview of registered users.
                            </p>
                        </div>
                        </div>
                    </div>
                    <div class="w-full px-4 md:w-1/2 lg:w-1/3">
                        <div class="mx-auto mb-10 max-w-[370px]">
                        <div class="mb-8 overflow-hidden rounded">
                            <img
                            src="https://cdn.discordapp.com/attachments/923643835073060886/1043583421953363978/image.png?ex=65ac074c&is=6599924c&hm=af8beca125c685a75c772db3d0f612bb67b2c0c970e2ad7e8c698266cb3d2cf4&"
                            alt="image"
                            class="w-full"
                            />
                        </div>
                        <div>
                            <h3>
                            <a
                                href="javascript:void(0)"
                                class="text-dark hover:text-primary mb-4 inline-block text-xl font-semibold sm:text-2xl lg:text-xl xl:text-2xl"
                            >
                                Web Application Development
                            </a>
                            </h3>
                            <p class="text-body-color text-base">
                              Design and development of a web application for fast and efficient order processing including CRUD functionalities (login/registration).
                            </p>
                        </div>
                        </div>
                    </div>
                    <div class="w-full px-4 md:w-1/2 lg:w-1/3">
                        <div class="mx-auto mb-10 max-w-[370px]">
                        <div class="mb-8 overflow-hidden rounded">
                            <img
                            src="https://cdn.discordapp.com/attachments/997826356639453245/1025522716113109002/unknown.png?ex=65b426f4&is=65a1b1f4&hm=772706b5e84d1dfaa931c7d2d0d952f659cf799c79cfbbc03cd027e9df174abc&"
                            alt="image"
                            class="w-120 h-100"
                            />
                        </div>
                        <div>
                            <h3>
                            <a
                                href="javascript:void(0)"
                                class="text-dark hover:text-primary mb-4 inline-block text-xl font-semibold sm:text-2xl lg:text-xl xl:text-2xl"
                            >
                                Website Deployment
                            </a>
                            </h3>
                            <p class="text-body-color text-base">
                                 Successful deployment and configuration of a finished website to a ubuntu server environment.
                            </p>
                        </div>
                        </div>
                    </div>
                    <div class="w-full px-4 md:w-1/2 lg:w-1/3">
                        <div class="mx-auto mb-10 max-w-[370px]">
                        <div class="mb-8 overflow-hidden rounded">
                            <img
                            src="https://cdn.discordapp.com/attachments/923643835073060886/1043282153825386506/image.png?ex=65b42938&is=65a1b438&hm=33fe40570d48b94a7b05a6bd11728151a34e2c422a030fd0e7ac01a043a555ea&"
                            alt="image"
                            class="w-120"
                            />
                        </div>
                        <div>
                            <h3>
                            <a
                                href="javascript:void(0)"
                                class="text-dark hover:text-primary mb-4 inline-block text-xl font-semibold sm:text-2xl lg:text-xl xl:text-2xl"
                            >
                                CRUD Implementation
                            </a>
                            </h3>
                            <p class="text-body-color text-base">
                                Addition of CRUD functionalities to an existing web application powering user management and administration.
                            </p>
                        </div>
                        </div>
                    </div>


                    </div>
                </div>
                </section>

        <footer class="bg-cyan-900 mt-8">
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

</style>
