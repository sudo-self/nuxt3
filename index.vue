useSeoMeta({
  title: 'nuxt3',
  description: 'A nuxt3 and tailwind.css website boilerplate written in typescript',
  ogTitle: 'nuxt3',
  ogDescription: '[og:description]',
  ogImage: '[og:image]',
  ogUrl: 'https://nuxt3.jessejesse.com',
  twitterTitle: 'iLostmyipad',
  twitterDescription: '[twitter:description]',
  twitterImage: '[twitter:image]',
  twitterCard: 'summary'
})

useHead({
  htmlAttrs: {
    lang: 'en'
  },
  link: [
    {
      rel: 'icon',
      type: 'image/png',
      href: '/favicon.png'
    }
  ]
})

<template>
  <div class="wrapper">
    <div class="margins" style="padding-top: 3rem; ">
      <div class="content">
        <h1 class="heading">
          Welcome to&nbsp;<span class="gradient__text">Your Website Name Here</span>&nbsp;
        </h1>
        <p class="description">
         &nbsp;<span class="gradient__text"> Nuxt.js</span>&nbsp An open-source Javascript framework.
        </p>
      </div>

      <div class="modules_grid">
      </div>
    </div>


    <div class="margins footer">
      <div style="color: #D1D5DB">
              
        <NuxtLink href="https://JesseJesse.com" target="_blank" class="hover-underline-animation">
        <span class="gradient__text">JesseJesse.com</span>
        </NuxtLink>
      </div>
      <div class="social">
              <NuxtLink href="https://nuxt3.jessejesse.com" target="_blank" class="hover-underline-animation">
                  <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 64 64"><path fill="#93bbc5" d="M63.361 21.857C63.361 9.778 49.634 0 32.681 0C15.729 0 2 9.778 2 21.857c0 12.067 13.729 41.832 30.681 41.832c16.953-.001 30.68-29.765 30.68-41.832"></path><path fill="#25333a" d="M23.983 28.554c6.687 9.148 9.1 18.74 5.407 21.445c-3.704 2.704-12.11-2.512-18.794-11.659c-6.68-9.14-9.107-18.739-5.405-21.448c3.698-2.701 12.11 2.527 18.792 11.662"></path><path fill="#d1d2d2" d="M19.557 29.02c3.89 5.323 5.294 10.904 3.147 12.479c-2.156 1.574-7.04-1.462-10.936-6.782c-3.888-5.321-5.299-10.904-3.145-12.483c2.151-1.57 7.05 1.472 10.934 6.786"></path><path fill="#25333a" d="M41.21 28.554c-6.688 9.148-9.1 18.74-5.407 21.445c3.704 2.704 12.11-2.512 18.794-11.659c6.681-9.14 9.107-18.739 5.405-21.448c-3.698-2.701-12.12 2.527-18.792 11.662"></path><path fill="#d1d2d2" d="M46.11 28.999c-3.89 5.321-5.295 10.904-3.146 12.478c2.154 1.572 7.04-1.461 10.937-6.786c3.886-5.316 5.299-10.902 3.145-12.478c-2.152-1.571-7.05 1.469-10.936 6.786"></path></svg>        </NuxtLink>
        <NuxtLink href="https://twitter.com/ilostmyipad" target="_blank" class="hover-underline-animation">
                 <span class="gradient__text">@iLostmyipad</span>
        </NuxtLink>
      </div>
    </div>
  </div>
</template>
<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica,
    Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
    background-color: #eefbfc;
    color: #484848;
  }

  /* Layout */
  .wrapper {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    width: 100%;
    min-height: 100vh;
    color: #ffffff;
    background-color: #0E0E10;
  }
  .margins {
    padding-left: 1rem;
    padding-right: 1rem;

    @media (min-width: 1024px) {
      padding-left: 5rem;
      padding-right: 5rem;
    }
  }

  /* Heading */
  .content {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
  }
  .content .heading {
    font-size: 2.4rem;
    line-height: 2.25rem;
    font-weight: 700;

    @media (min-width: 1280px) {
      font-size: 3rem;
      line-height: 1;
    }
  }

  .content .description {
    font-size: 1.125rem;
    line-height: 1.75rem;
    color: #9CA3AF;

    @media (min-width: 1280px) {
      font-size: 1.25rem;
      line-height: 1.75rem;
    }
  }

  /* Modules */
  .modules_grid {
    display: grid;
    margin-top: 2.5rem;
    gap: 2rem;

    @media (min-width: 768px) {
      grid-template-columns: repeat(2, minmax(0, 1fr));
    }

    @media (min-width: 1280px) {
      grid-template-columns: repeat(3, minmax(0, 1fr));
    }
  }
  .card {
    position: relative;
    padding: 30px;
    border-radius: 10px;
    transition: 0.5s;
    box-shadow: inset 5px 5px 5px rgba(0, 0, 0, 0.2),
    inset -5px -5px 15px rgba(255, 255, 255, 0.1),
    5px 5px 15px rgba(0, 0, 0, 0.3), -5px -5px 15px rgba(255, 255, 255, 0.1);
  }

  .card .layout {
    display: flex;
    flex-direction: column;
    gap: 2rem;
    justify-content: space-between;
    height: 100%;
  }

  .card .layout .group {
    display: flex;
    flex-direction: column;
    gap: 0.75rem;
  }

  .card .layout .heading {
    font-size: 1.5rem;
    line-height: 2rem;
    font-weight: 700;
  }

  .card .layout .description {
    color: #D1D5DB;
  }

  .card .layout .group .actions {
    display: flex;
    gap: 0.5rem;
  }

  /* Footer */
  .footer {
    display: flex;
    padding-top: 1rem;
    padding-bottom: 1rem;
    margin-top: 2.5rem;
    justify-content: space-between;
    align-items: center;
    border-top-width: 1px;
    border-color: #1F2937;
    width: 100%;
  }

  .footer .social {
    display: flex;
    gap: 1.25rem;
    align-items: center;
  }

  /* Special */
  .gradient__text {
    background: linear-gradient(to right, #7bceb6 10%, #12a87b 40%, #0FCF97 60%, #7bceb6 90%);
    background-size: 200% auto;
    color: #000;
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    animation: shine 1s linear infinite;
  }

  @keyframes shine {
    to {
      background-position: 200% center;
    }
  }
  .hover-underline-animation {
    display: inline-block;
    position: relative;
    color: #5BF3C7;
    text-decoration: none;
  }

  .hover-underline-animation::after {
    content: '';
    position: absolute;
    width: 100%;
    transform: scaleX(0);
    height: 2px;
    bottom: 0;
    left: 0;
    background-color: #5BF3C7;
    transform-origin: bottom right;
    transition: transform 0.25s ease-out;
  }

  .hover-underline-animation:hover::after {
    transform: scaleX(1);
    transform-origin: bottom left;
  }
</style>
