<template>
  <!-- Featured articles  -->
  <section class="featured-articles section section-header-offset">
    <div class="featured-articles-container container d-grid">
      <div class="featured-content d-grid">
        <div class="headline-banner">
          <h3 class="headline fancy-border">
            <span class="place-items-center">Breaking news</span>
          </h3>
          <span class="headline-description">Apple announces a new partnership...</span>
        </div>

        <a href="./post.html" class="article featured-article featured-article-1">
          <img src="./../../assets/images/featured/featured-1.jpg" alt="" class="article-image" />
          <span class="article-category">Technology</span>

          <div class="article-data-container">
            <div class="article-data">
              <span>Dec 5th 2021</span>
              <span class="article-data-spacer"></span>
              <span>8 Min read</span>
            </div>

            <h3 class="title article-title">Is VR the future?</h3>
          </div>
        </a>

        <a href="./post.html" class="article featured-article featured-article-2">
          <img src="./../../assets/images/featured/featured-2.jpg" alt="" class="article-image" />
          <span class="article-category">Food</span>

          <div class="article-data-container">
            <div class="article-data">
              <span>Dec 6th 2021</span>
              <span class="article-data-spacer"></span>
              <span>4 Min read</span>
            </div>

            <h3 class="title article-title">Fine dining 101</h3>
          </div>
        </a>

        <a href="./post.html" class="article featured-article featured-article-3">
          <img src="./../../assets/images/featured/featured-3.jpg" alt="" class="article-image" />
          <span class="article-category">Health</span>

          <div class="article-data-container">
            <div class="article-data">
              <span>Dec 5th 2021</span>
              <span class="article-data-spacer"></span>
              <span>5 Min read</span>
            </div>

            <h3 class="title article-title">Natural fat burner</h3>
          </div>
        </a>
      </div>

      <div class="sidebar d-grid">
        <h3 class="title featured-content-title">Trending news</h3>

        <a href="#" class="trending-news-box">
          <div class="trending-news-img-box">
            <span class="trending-number place-items-center">01</span>
            <img src="./../../assets/images/trending/trending_1.jpg" alt="" class="article-image" />
          </div>

          <div class="trending-news-data">
            <div class="article-data">
              <span>23 Dec 2021</span>
              <span class="article-data-spacer"></span>
              <span>3 Min read</span>
            </div>

            <h3 class="title article-title">Sample article title</h3>
          </div>
        </a>

        <a href="#" class="trending-news-box">
          <div class="trending-news-img-box">
            <span class="trending-number place-items-center">02</span>
            <img src="./../../assets/images/trending/trending_2.jpg" alt="" class="article-image" />
          </div>

          <div class="trending-news-data">
            <div class="article-data">
              <span>23 Dec 2021</span>
              <span class="article-data-spacer"></span>
              <span>3 Min read</span>
            </div>

            <h3 class="title article-title">Sample article title</h3>
          </div>
        </a>

        <a href="#" class="trending-news-box">
          <div class="trending-news-img-box">
            <span class="trending-number place-items-center">03</span>
            <img src="./../../assets/images/trending/trending_3.jpg" alt="" class="article-image" />
          </div>

          <div class="trending-news-data">
            <div class="article-data">
              <span>23 Dec 2021</span>
              <span class="article-data-spacer"></span>
              <span>3 Min read</span>
            </div>

            <h3 class="title article-title">Sample article title</h3>
          </div>
        </a>

        <a href="#" class="trending-news-box">
          <div class="trending-news-img-box">
            <span class="trending-number place-items-center">04</span>
            <img src="./../../assets/images/trending/trending_4.jpg" alt="" class="article-image" />
          </div>

          <div class="trending-news-data">
            <div class="article-data">
              <span>23 Dec 2021</span>
              <span class="article-data-spacer"></span>
              <span>3 Min read</span>
            </div>

            <h3 class="title article-title">Sample article title</h3>
          </div>
        </a>

        <a href="#" class="trending-news-box">
          <div class="trending-news-img-box">
            <span class="trending-number place-items-center">05</span>
            <img src="./../../assets/images/trending/trending_5.jpg" alt="" class="article-image" />
          </div>

          <div class="trending-news-data">
            <div class="article-data">
              <span>23 Dec 2021</span>
              <span class="article-data-spacer"></span>
              <span>3 Min read</span>
            </div>

            <h3 class="title article-title">Sample article title</h3>
          </div>
        </a>
      </div>
    </div>
  </section>
</template>

<style>
/* Featured articles */
.featured-articles {
  padding-block: 2rem;
}

.section-header-offset {
  margin-top: 7.4rem;
}

.featured-articles-container,
.featured-content {
  gap: var(--gap);
}

.headline-banner {
  background-color: var(--secondary-background-color);
  display: flex;
  align-items: center;
  gap: var(--gap);
  font-size: var(--font-size-xsm);
}

.headline {
  background-color: #000;
  color: var(--light-color);
  font-size: 1rem;
  text-transform: uppercase;
  text-align: center;
  letter-spacing: 1px;
  padding: 4px;
  height: 100%;
}

.headline span {
  height: inherit;
}

.fancy-border {
  position: relative;
  overflow: hidden;
}

.fancy-border::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 200%;
  height: 100%;
  background: var(--gradient-color);
  background-size: 50% 100%;
  z-index: 5;
}

.fancy-border span {
  position: relative;
  z-index: 10;
  display: inline-flex;
  background-color: var(--secondary-background-color);
  padding: 0.6rem 1.5rem;
}

.article {
  position: relative;
  min-height: var(--item-min-height-md);
}

.article-image {
  position: absolute;
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.25s;
}

.article-category {
  position: absolute;
  top: 1rem;
  right: 1rem;
  padding: 1rem;
  background-color: var(--primary-background-color);
  font-size: 1rem;
  color: var(--light-color);
  text-transform: uppercase;
  z-index: 10;
}

.article-data-container {
  width: 100%;
  position: absolute;
  left: 0;
  bottom: 0;
  padding: 2rem 1.5rem;
  background-color: var(--transparent-dark-color);
  z-index: 10;
  transition: background-color 0.5s;
}

/* Light theme color hover styles */
.article:hover .article-data-container {
  background-color: var(--hover-dark-color);
  color: var(--hover-light-color);
}

.article:hover .article-data-spacer {
  background-color: var(--hover-light-color);
}

.article:hover .article-title {
  color: var(--hover-light-color);
}

.article-data {
  display: flex;
  align-items: center;
  gap: var(--gap);
  font-size: var(--font-size-xsm);
  margin-bottom: 1rem;
}

.article-data-spacer {
  width: 0.5rem;
  height: 0.5rem;
  background-color: var(--light-color-alt);
  transform: rotate(45deg);
}

.title {
  color: var(--light-color);
}

.article-title {
  font-size: var(--font-size-md);
}

/* Sidebar */
.sidebar {
  background-color: var(--secondary-background-color);
  padding: 2.5rem;
}

.trending-news-box {
  display: flex;
  flex-direction: column;
  gap: var(--gap);
  padding-block: 2rem;
  border-bottom: 1px solid var(--transparent-light-color);
}

.trending-news-box:last-of-type {
  border-bottom: none;
}

.featured-content-title {
  font-size: var(--font-size-md);
  text-align: center;
  padding: 1rem;
}

.trending-news-img-box {
  position: relative;
  width: 100%;
  height: var(--item-min-height-sm);
}

.trending-number {
  position: absolute;
  top: -1rem;
  left: -1rem;
  z-index: 15;
  width: 3rem;
  height: 3rem;
  background-color: var(--secondary-background-color);
  color: var(--light-color);
  border-radius: 50%;
}

.trending-news-data .article-title {
  font-size: var(--font-size-sm);
}

.trending-news-box:hover .article-title {
  color: var(--light-color-alt);
}
</style>