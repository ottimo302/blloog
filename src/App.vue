<script>
import TheHeader from './components/header/TheHeader.vue'
import ArticlesMain from './components/articles/ArticlesMain.vue'
import OlderPosts from './components/articles/OlderPosts.vue'
import PopularTags from './components/articles/PopularTags.vue'
import TheFooter from './components/footer/TheFooter.vue'

export default {
  components: {
    TheHeader,
    ArticlesMain,
    OlderPosts,
    PopularTags,
    TheFooter
  }
}
</script>

<template>
  <div>
    <TheHeader></TheHeader>
    <ArticlesMain></ArticlesMain>
    <OlderPosts></OlderPosts>
    <PopularTags></PopularTags>
    <TheFooter></TheFooter>
  </div>
</template>

<style>
/* Import font */
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap');

/* Custom properties */
:root {
  --light-color: #fff;
  --light-color-alt: #afb6cd;
  --primary-background-color: #131417;
  --secondary-background-color: #252830;
  --hover-light-color: var(--light-color);
  --hover-dark-color: var(--primary-background-color);
  --gradient-color: linear-gradient(115deg, #4fcf70, #fad648, #a767e5, #12bcfe, #44ce7b);
  --transparent-light-color: rgba(255, 255, 255, 0.05);
  --transparent-dark-color: rgba(0, 0, 0, 0.75);
  --font-family: 'Poppins', sans-serif;
  --font-size-xsm: 1.2rem;
  --font-size-sm: 1.6rem;
  --font-size-md: 2.4rem;
  --font-size-lg: 3rem;
  --font-size-xl: 4rem;
  --gap: 2rem;
  --margin-sm: 2rem;
  --margin-md: 3rem;
  --item-min-height-sm: 20rem;
  --item-min-height-md: 30rem;
}

/* Base styles */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  font-size: 62.5%;
}

body {
  font-family: var(--font-family);
  font-size: var(--font-size-sm);
  color: var(--light-color-alt);
  background-color: var(--primary-background-color);
  letter-spacing: 1px;
  transition: background-color 0.25s, color 0.25s;
}

a {
  color: inherit;
  text-decoration: none;
}

ul {
  list-style: none;
}

img {
  max-width: 100%;
}

input,
button {
  font: inherit;
  color: inherit;
  border: none;
  background-color: transparent;
}

i {
  font-size: var(--font-size-md);
}
/* Theme color change */
body.light-theme {
  --light-color: #3d3d3d;
  --light-color-alt: rgba(0, 0, 0, 0.6);
  --primary-background-color: #fff;
  --secondary-background-color: #f1f1f1;
  --hover-light-color: #fff;
  --transparent-dark-color: var(--secondary-background-color);
  --transparent-light-color: rgba(0, 0, 0, 0.1);
}
/* Reusable classes */
.container {
  max-width: 160rem;
  margin: 0 auto;
  padding: 0 1.5rem;
}

.place-items-center {
  display: inline-flex;
  align-items: center;
  justify-content: center;
}

.section:not(.featured-articles) {
  padding-block: 5rem;
}

.d-grid {
  display: grid;
}

.screen-sm-hidden {
  display: none;
}

@media screen and (min-width: 700px) {
  .trending-news-box {
    flex-direction: row;
    align-items: center;
  }

  .trending-news-img-box {
    width: 50%;
  }

  .trending-news-data {
    margin: auto;
    text-align: center;
  }

  .newsletter-description {
    max-width: 40rem;
  }

  .form-container-inner {
    align-items: center;
  }

  .popular-tags-container,
  .footer-container {
    grid-template-columns: repeat(2, 1fr);
  }

  .company-data {
    order: 0;
  }

  .author {
    grid-template-columns: 25rem 1fr;
  }
}

@media screen and (min-width: 768px) {
  .featured-content {
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: 5rem repeat(4, 1fr);
  }

  .headline-banner {
    grid-column: 1/-1;
    font-size: var(--font-size-sm);
  }

  .featured-article {
    grid-column: 3/-1;
    grid-row: 2/4;
  }

  .featured-article-1 {
    grid-column: 1/3;
  }

  .featured-article-3 {
    grid-column: 1/-1;
    grid-row: 4/6;
  }

  .older-posts .article {
    grid-template-columns: 25rem 1fr;
  }

  .older-posts-article-image-wrapper {
    height: auto;
  }

  .blog-post-data img {
    height: var(--item-min-height-md);
  }
}

@media screen and (min-width: 1024px) {
  .menu {
    position: static !important;
    width: initial !important;
    padding: initial !important;
    background-color: transparent !important;
    opacity: 1 !important;
    transform: scale(1) !important;
  }

  .menu > .list {
    flex-direction: row !important;
  }

  .screen-lg-hidden {
    display: none;
  }

  .screen-sm-hidden {
    display: block;
  }

  .sign-up-btn {
    padding: 4px;
  }

  /* Fancy button animation effect */
  .btn.fancy-border:hover::before {
    animation: animate_border 0.75s linear infinite;
  }

  @keyframes animate_border {
    to {
      transform: translateX(-50%);
    }
  }

  .featured-articles-container {
    grid-template-columns: 1fr 40rem;
  }

  .trending-news-img-box {
    width: 10rem;
    height: 10rem;
  }

  .popular-tags-container {
    grid-template-columns: repeat(3, 1fr);
  }

  .footer-container {
    grid-template-columns: repeat(5, 1fr);
  }

  .company-data {
    grid-column: span 2;
  }

  .company-description {
    max-width: 85%;
  }

  .copyright-notice {
    margin-top: auto;
  }

  .blog-post-data img {
    height: 40rem;
  }
}

@media screen and (min-width: 1200px) {
  .older-posts-grid-wrapper {
    grid-template-columns: repeat(2, 1fr);
  }
}
@media screen and (min-width: 1500px) {
  .featured-article {
    grid-column: 3/-1;
  }

  .featured-article-1 {
    grid-column: 1/3;
    grid-row: 2/-1;
  }
}
</style>
