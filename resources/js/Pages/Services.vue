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



                <div x-data="{
                    billingType: 'month',
                    basicPrice: '19',
                    premiumPrice: '29',
                    proPrice: '39'
                }" class="min-h-full bg-gray-100 pb-12 pt-16">
                <div class="w-full bg-gray-100 pt-16 pb-24 text-center">
                    <h1 class="sm:mx-auto sm:w-10/12 md:w-2/3 font-black text-cyan-900 text-4xl text-center sm:text-5xl md:text-6xl lg:w-auto lg:text-center xl:text-7xl">Experience Digital Excellence</h1>
                    <h4 class="text-2xl text-black mt-6">Choose the right plan for you</h4>
                    <p class="text-md text-black mt-1">All packages come with active support and communication upon hand-over.</p>
                    <div class="flex items-center justify-center mt-8">
                        <button @click="
                                billingType = 'month',
                                basicPrice = '19',
                                premiumPrice = '29',
                                proPrice = '39'
                            " class="text-gray-800 px-4 py-2 rounded-tl-lg rounded-bl-lg bg-gray-200" :class=" billingType === 'month' ? 'bg-blue-300' : 'bg-gray-200' " title="Choose Monthly billing">
                            One-time Billing
                        </button>
                        <button @click="
                                billingType = 'year',
                                basicPrice = '205',
                                premiumPrice = '313',
                                proPrice = '421'
                            " class="text-gray-800 px-4 py-2 rounded-tr-lg rounded-br-lg bg-gray-200" :class=" billingType === 'year' ? 'bg-blue-300' : 'bg-gray-200' " title="Choose Annual billing">
                            Hourly/Fixed Billing
                        </button>
                    </div>
                </div>
                <div class="w-full 2xl:w-3/4 flex items-center justify-center px-8 md:px-32 lg:px-16 2xl:px-0 mx-auto -mt-8">
                    <div class="w-full grid grid-cols-1 xl:grid-cols-3 gap-8">
                        <div class="bg-white shadow-2xl rounded-lg py-4">
                            <p class="text-4xl text-center font-bold text-cyan-800 font-serif">Website</p>
                            <!--<p class="text-lg text-center text-gray-500"><a href="https://jumpshare.com/s/kmXtoSixGT4EU4fBqvMT">Example</a></p>-->
                            <p class="text-sm text-center text-gray-500 uppercase mt-3"><a href="https://jumpshare.com/s/kmXtoSixGT4EU4fBqvMT">starting at:</a></p>
                            <p class="text-center mb-2">
                                <span class="text-4xl font-bold text-gray-700">
                                    <span x-text="basicPrice">€189.99</span>
                                </span>
                                <span class="text-xs uppercase text-gray-500">
                                    / <span x-text="billingType">+ VAT</span>
                                </span>
                                <br/>
                                <a href="../"></a>
                            </p>
                            <!--<div class="pt-4 pb-4 flex gap-3 justify-center grayscale border-b border-t">
                            <img src="https://www.fullstackpython.com/img/logos/vuejs-wide.png" class="h-8 sm:h-10 w-auto lg:h-12" alt="" />
                            <img src="https://techalmas.com/wp-content/uploads/2021/02/Laravel_logo_wordmark_logotype.png" class="h-8 sm:h-10 w-auto lg:h-12" alt="" />
                            </div>-->
                            <ul class="border-gray-300 py-8 space-y-6">
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-800 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Single-page Application (SPA)*</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-800 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Multi-page Application (PWA/SSR)**</span>
                                </li>

                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-800 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Personalized Design</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-800 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Responsive & User-friendly</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-800 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Custom Functionalities**</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-800 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Contact Form</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-800 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Email Newsletter**</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-800 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Ready For Production</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-800 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Optimized For Performance**</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-800 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Active Support & consultations**</span>
                                </li>
                            </ul>
                            <div class="flex items-center justify-center mt-6">
                                <a href="/info" class="bg-cyan-900 hover:bg-cyan-700 px-8 py-2 text-sm text-white uppercase rounded font-bold transition duration-150" title="order">order now</a>
                            </div>
                        </div>

                        <div class="bg-white shadow-2xl rounded-lg py-4">
                            <p class="text-4xl text-center font-bold text-cyan-800 font-serif">Cloud Intergration</p>
                            <p class="text-sm text-center text-gray-500 uppercase mt-3"><a href="https://jumpshare.com/s/kmXtoSixGT4EU4fBqvMT">starting at:</a></p>
                            <p class="text-center mb-2">
                                <span class="text-4xl font-bold text-gray-700">
                                    <span x-text="basicPrice">€57.99</span>
                                </span>
                                <span class="text-xs uppercase text-gray-500">
                                    / <span x-text="billingType">+ VAT</span>
                                </span>
                                <br/>
                                <a href="../"></a>
                            </p>
                            <!--<div class="py-4 flex gap-2 text-center justify-center grayscale border-t border-b">
                                <span class="text-gray-600 capitalize">Vue/React + Laravel (HTML/CSS/JS/PHP)</span>
                                <span class="text-gray-600 capitalize">Ubuntu 20.04 + MySQL (DigitalOcean/cPanel)</span>
                            </div>-->
                            <ul class="border-gray-300 py-8 space-y-6">
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Node.js (Vue/React...) & Laravel (PHP)*</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">WordPress (PHP) & Others (HTML/CSS/JS...)*</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Project & Server Assessment (bugs, security...)**</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Environmental Configuration (proj. dependant)</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Domain/DNS Configurations (NGINX/SSL...)**</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Database Intergration (MariaDB/MySQL...)*</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">File-transfer access (via FTP client)</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">server environment Documentation</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Quality Assurance & Unit Testing (QA/UT)**</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Active Support & Consultations**</span>
                                </li>
                            </ul>
                            <div class="flex items-center justify-center mt-6">
                                <a href="/info" class="bg-cyan-900 hover:bg-cyan-700 px-8 py-2 text-sm text-white uppercase rounded font-bold transition duration-150" title="order">order now</a>
                            </div>
                        </div>

                        <div class="bg-white shadow-2xl rounded-lg py-4">
                            <p class="text-4xl text-center font-bold text-cyan-800 font-serif">Freelance Work</p>
                            <p class="text-sm text-center text-gray-500 uppercase mt-3"><a href="https://jumpshare.com/s/kmXtoSixGT4EU4fBqvMT">starting at:</a></p>
                            <p class="text-center mb-2">
                                <span class="text-4xl font-bold text-gray-700">
                                    <span x-text="basicPrice">€15.99</span>
                                </span>
                                <span class="text-xs uppercase text-gray-500">
                                    / <span x-text="billingType">hourly</span>
                                </span>
                                <br/>
                                <a href="../"></a>
                            </p>
                            <!--<div class="py-5 flex gap-2 text-center justify-center grayscale border-t border-b">
                                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3a/Logo-ubuntu_no%28r%29-black_orange-hex.svg/1280px-Logo-ubuntu_no%28r%29-black_orange-hex.svg.png" class="h-8 sm:h-10 w-auto lg:h-10" alt="" />
                                <img src="https://www.whmcs.com/assets/images/cpanel/cpanel-logo-lg.png" class="h-8 sm:h-10 w-auto lg:h-10" alt="" />
                            </div>-->
                            <ul class="border-gray-300 py-8 space-y-6">
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Full-stack development</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Database Administration (DBA)</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Systems Administration</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">long-term or short-term</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Upwards of 40hrs / weekly</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Job Success Rate: 100%</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Upwork avg. rating: 4.85 (2)</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Open to work on various projects</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Reliable and Flexible Work schedule</span>
                                </li>
                                <li class="flex items-center space-x-2 px-8">
                                    <span class="bg-cyan-900 rounded-full p-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-3 w-3 text-white" viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
                                        </svg>
                                    </span>
                                    <span class="text-gray-600 capitalize">Work Terms: freelancer via <a class="text-blue-700" href="https://www.upwork.com/freelancers/~01e0ea10215a43ee5a">Upwork</a></span>
                                </li>
                            </ul>
                            <div class="flex items-center justify-center mt-6">
                                <a href="/info" class="bg-cyan-900 hover:bg-cyan-700 px-8 py-2 text-sm text-white uppercase rounded font-bold transition duration-150" title="order">order now</a>
                            </div>
                        </div>
                    </div>
                </div>
        </div>

        <footer class="bg-cyan-900">
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
