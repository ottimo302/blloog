<template>
  <!-- Footer -->
  <footer class="footer section">
    <div class="footer-container container d-grid">
      <div class="company-data">
        <a href="./index.html">
          <h2 class="logo">NewsFlash</h2>
        </a>
        <p class="company-description">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere, iure. Harum, animi
          dolores, nam, ad magni expedita.
        </p>

        <ul class="list social-media">
          <li class="list-item">
            <a href="#" class="list-link"><i class="ri-instagram-line"></i></a>
          </li>
          <li class="list-item">
            <a href="#" class="list-link"><i class="ri-facebook-circle-line"></i></a>
          </li>
          <li class="list-item">
            <a href="#" class="list-link"><i class="ri-twitter-line"></i></a>
          </li>
          <li class="list-item">
            <a href="#" class="list-link"><i class="ri-pinterest-line"></i></a>
          </li>
        </ul>

        <span class="copyright-notice">&copy;2021 NewsFlash. All rights reserved.</span>
      </div>

      <div>
        <h6 class="title footer-title">Categories</h6>

        <ul class="footer-list list">
          <li class="list-item">
            <a href="#" class="list-link">Travel</a>
          </li>
          <li class="list-item">
            <a href="#" class="list-link">Food</a>
          </li>
          <li class="list-item">
            <a href="#" class="list-link">Technology</a>
          </li>
          <li class="list-item">
            <a href="#" class="list-link">Health</a>
          </li>
          <li class="list-item">
            <a href="#" class="list-link">Nature</a>
          </li>
          <li class="list-item">
            <a href="#" class="list-link">Fitness</a>
          </li>
        </ul>
      </div>

      <div>
        <h6 class="title footer-title">Useful links</h6>

        <ul class="footer-list list">
          <li class="list-item">
            <a href="#" class="list-link">Home</a>
          </li>
          <li class="list-item">
            <a href="#" class="list-link">Elements</a>
          </li>
          <li class="list-item">
            <a href="#" class="list-link">Tags</a>
          </li>
          <li class="list-item">
            <a href="#" class="list-link">Authors</a>
          </li>
          <li class="list-item">
            <a href="#" class="list-link">Membership</a>
          </li>
        </ul>
      </div>

      <div>
        <h6 class="title footer-title">Company</h6>

        <ul class="footer-list list">
          <li class="list-item">
            <a href="#" class="list-link">Contact us</a>
          </li>
          <li class="list-item">
            <a href="#" class="list-link">F.A.Q</a>
          </li>
          <li class="list-item">
            <a href="#" class="list-link">Careers</a>
          </li>
          <li class="list-item">
            <a href="#" class="list-link">Authors</a>
          </li>
          <li class="list-item">
            <a href="#" class="list-link">Memberships</a>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<style>
/* Footer */
.footer {
  background-color: var(--secondary-background-color);
}

.footer-container {
  gap: var(--gap);
}

.company-data {
  display: flex;
  flex-direction: column;
  order: 1;
}

.company-description {
  margin-block: var(--margin-sm);
  max-width: 75%;
}

.social-media {
  margin-bottom: var(--margin-md);
}

.copyright-notice {
  opacity: 0.8;
}

.footer-list {
  flex-direction: column;
  align-items: flex-start;
}

.footer-title {
  font-size: var(--font-size-sm);
  text-transform: uppercase;
  margin-bottom: var(--margin-sm);
}

/* Scrollbar */
::-webkit-scrollbar {
  width: 1rem;
}

::-webkit-scrollbar-track {
  background: #f1f1f1;
}

::-webkit-scrollbar-thumb {
  background: #3f4254;
}

::-webkit-scrollbar-thumb:hover {
  background: #2e303b;
}
</style>