<template>
  <!-- Popular tags -->
  <section class="popular-tags section">
    <div class="container">
      <h2 class="title section-title" data-name="Popular tags">Popular tags</h2>

      <div class="popular-tags-container d-grid">
        <a href="#" class="article">
          <span class="tag-name">#Travel</span>
          <img src="./../../assets/images/tags/travel-tag.jpg" alt="" class="article-image" />
        </a>

        <a href="#" class="article">
          <span class="tag-name">#Food</span>
          <img src="./../../assets/images/tags/food-tag.jpg" alt="" class="article-image" />
        </a>

        <a href="#" class="article">
          <span class="tag-name">#Technology</span>
          <img src="./../../assets/images/tags/technology-tag.jpg" alt="" class="article-image" />
        </a>

        <a href="#" class="article">
          <span class="tag-name">#Health</span>
          <img src="./../../assets/images/tags/health-tag.jpg" alt="" class="article-image" />
        </a>

        <a href="#" class="article">
          <span class="tag-name">#Nature</span>
          <img src="./../../assets/images/tags/nature-tag.jpg" alt="" class="article-image" />
        </a>

        <a href="#" class="article">
          <span class="tag-name">#Fitness</span>
          <img src="./../../assets/images/tags/fitness-tag.jpg" alt="" class="article-image" />
        </a>
      </div>
    </div>
  </section>
</template>

<style>
/* Popular tags */
.popular-tags-container {
  gap: var(--gap);
}

.popular-tags-container .article {
  min-height: var(--item-min-height-sm);
}

.tag-name {
  padding: 1rem 2rem;
  background-color: var(--transparent-dark-color);
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  z-index: 10;
}

.popular-tags-container .article:hover .tag-name {
  color: var(--light-color);
}

.popular-tags-container .article {
  overflow: hidden;
}

.popular-tags-container .article:hover .article-image {
  transform: scale(1.05);
}
</style>