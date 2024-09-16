<template>
  <!-- Older posts -->
  <section class="older-posts section">
    <div class="container">
      <h2 class="title section-title" data-name="Older posts">Older posts</h2>

      <div class="older-posts-grid-wrapper d-grid">
        <a href="#" class="article d-grid">
          <div class="older-posts-article-image-wrapper">
            <img
              src="./../../assets/images/older_posts/older_posts_1.jpg"
              alt=""
              class="article-image"
            />
          </div>

          <div class="article-data-container">
            <div class="article-data">
              <span>23 Dec 2021</span>
              <span class="article-data-spacer"></span>
              <span>3 Min read</span>
            </div>

            <h3 class="title article-title">Sample article title</h3>
            <p class="article-description">
              Lorem, ipsum dolor sit amet consectetur adipisicing elit. Similique a tempore sapiente
              corporis, eaque fuga placeat odit voluptatibus.
            </p>
          </div>
        </a>

        <a href="#" class="article d-grid">
          <div class="older-posts-article-image-wrapper">
            <img
              src="./../../assets/images/older_posts/older_posts_2.jpg"
              alt=""
              class="article-image"
            />
          </div>

          <div class="article-data-container">
            <div class="article-data">
              <span>23 Dec 2021</span>
              <span class="article-data-spacer"></span>
              <span>3 Min read</span>
            </div>

            <h3 class="title article-title">Sample article title</h3>
            <p class="article-description">
              Lorem, ipsum dolor sit amet consectetur adipisicing elit. Similique a tempore sapiente
              corporis, eaque fuga placeat odit voluptatibus.
            </p>
          </div>
        </a>

        <a href="#" class="article d-grid">
          <div class="older-posts-article-image-wrapper">
            <img
              src="./../../assets/images/older_posts/older_posts_3.jpg"
              alt=""
              class="article-image"
            />
          </div>

          <div class="article-data-container">
            <div class="article-data">
              <span>23 Dec 2021</span>
              <span class="article-data-spacer"></span>
              <span>3 Min read</span>
            </div>

            <h3 class="title article-title">Sample article title</h3>
            <p class="article-description">
              Lorem, ipsum dolor sit amet consectetur adipisicing elit. Similique a tempore sapiente
              corporis, eaque fuga placeat odit voluptatibus.
            </p>
          </div>
        </a>

        <a href="#" class="article d-grid">
          <div class="older-posts-article-image-wrapper">
            <img
              src="./../../assets/images/older_posts/older_posts_4.jpg"
              alt=""
              class="article-image"
            />
          </div>

          <div class="article-data-container">
            <div class="article-data">
              <span>23 Dec 2021</span>
              <span class="article-data-spacer"></span>
              <span>3 Min read</span>
            </div>

            <h3 class="title article-title">Sample article title</h3>
            <p class="article-description">
              Lorem, ipsum dolor sit amet consectetur adipisicing elit. Similique a tempore sapiente
              corporis, eaque fuga placeat odit voluptatibus.
            </p>
          </div>
        </a>

        <a href="#" class="article d-grid">
          <div class="older-posts-article-image-wrapper">
            <img
              src="./../../assets/images/older_posts/older_posts_5.jpg"
              alt=""
              class="article-image"
            />
          </div>

          <div class="article-data-container">
            <div class="article-data">
              <span>23 Dec 2021</span>
              <span class="article-data-spacer"></span>
              <span>3 Min read</span>
            </div>

            <h3 class="title article-title">Sample article title</h3>
            <p class="article-description">
              Lorem, ipsum dolor sit amet consectetur adipisicing elit. Similique a tempore sapiente
              corporis, eaque fuga placeat odit voluptatibus.
            </p>
          </div>
        </a>

        <a href="#" class="article d-grid">
          <div class="older-posts-article-image-wrapper">
            <img
              src="./../../assets/images/older_posts/older_posts_6.jpg"
              alt=""
              class="article-image"
            />
          </div>

          <div class="article-data-container">
            <div class="article-data">
              <span>23 Dec 2021</span>
              <span class="article-data-spacer"></span>
              <span>3 Min read</span>
            </div>

            <h3 class="title article-title">Sample article title</h3>
            <p class="article-description">
              Lorem, ipsum dolor sit amet consectetur adipisicing elit. Similique a tempore sapiente
              corporis, eaque fuga placeat odit voluptatibus.
            </p>
          </div>
        </a>
      </div>

      <div class="see-more-container">
        <a href="#" class="btn see-more-btn place-items-center"
          >See more <i class="ri-arrow-right-s-line"></i
        ></a>
      </div>
    </div>
  </section>
</template>

<style>
/* Older posts */
.older-posts-grid-wrapper {
  gap: var(--gap);
}

.older-posts-article-image-wrapper,
.older-posts .article {
  min-height: var(--item-min-height-sm);
}

.older-posts .article {
  background-color: var(--secondary-background-color);
}

.older-posts-article-image-wrapper {
  position: relative;
}

.older-posts-grid-wrapper .article-data-container {
  position: static;
  background-color: transparent;
}

.older-posts-grid-wrapper .article-title {
  margin-bottom: var(--margin-sm);
}

.see-more-container {
  padding-top: var(--margin-md);
}

.see-more-btn {
  text-transform: uppercase;
}

.see-more-btn:hover {
  color: var(--light-color);
}

.see-more-btn i {
  transition: transform 0.25s;
}

.see-more-btn:hover i {
  transform: translateX(0.5rem);
}
</style>