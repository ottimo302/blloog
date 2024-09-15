<template>
  <!-- Header -->
  <header class="header" id="header">
    <nav class="navbar container">
      <!-- Header Logo -->
      <a href="./index.html">
        <h2 class="logo">blloog</h2>
      </a>

      <!-- Header-Links -->
      <div class="menu" id="menu">
        <ul class="list">
          <HeaderLinks
            v-for="linkData in linksData"
            :key="linkData.id"
            :classs="linkData.classs"
            :item="linkData.value"
          ></HeaderLinks>
        </ul>
      </div>

      <!-- Header Right Icons -->
      <div class="list list-right">
        <button class="btn place-items-center" id="theme-toggle-btn">
          <i class="ri-sun-line sun-icon"></i>
          <i class="ri-moon-line moon-icon"></i>
        </button>

        <button class="btn place-items-center" id="search-icon">
          <i class="ri-search-line"></i>
        </button>

        <button
          class="btn place-items-center screen-lg-hidden menu-toggle-icon"
          id="menu-toggle-icon"
        >
          <i class="ri-menu-3-line open-menu-icon"></i>
          <i class="ri-close-line close-menu-icon"></i>
        </button>

        <a href="#" class="list-link screen-sm-hidden">Sign in</a>
        <a href="#" class="btn sign-up-btn fancy-border screen-sm-hidden">
          <span>Sign up</span>
        </a>
      </div>
    </nav>
  </header>
</template>

<script>
import HeaderLinks from './HeaderLinks.vue'
export default {
  components: { HeaderLinks },
  data() {
    return {
      linksData: [
        {
          id: 'home',
          value: 'Home',
          classs: 'list-link'
        },
        {
          id: 'contact',
          value: 'Contact',
          classs: 'list-link'
        },
        {
          id: 'signin',
          value: 'Sign in',
          classs: 'list-item screen-lg-hidden'
        },
        {
          id: 'signup',
          value: 'Sign up',
          classs: 'list-item screen-lg-hidden'
        }
      ]
    }
  }
}
</script>

<style scoped>
/* Header */
.header {
  background-color: var(--secondary-background-color);
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 999;
}

.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding-block: 1.5rem;
}

.logo {
  font-size: var(--font-size-md);
  color: var(--light-color);
}

.menu {
  position: absolute;
  top: 8.5rem;
  right: 1.5rem;
  width: 23rem;
  padding: 1.5rem;
  background-color: var(--secondary-background-color);
  opacity: 0;
  transform: scale(0);
  transition: opacity 0.25s ease-in;
}

.list {
  display: flex;
  align-items: center;
  gap: var(--gap);
}

.menu > .list {
  flex-direction: column;
}

.list-link.current {
  color: var(--light-color);
}

.close-menu-icon {
  display: none;
}

.btn {
  cursor: pointer;
}

.list-link:hover,
.btn:hover,
.btn:hover span {
  color: var(--light-color);
}

.moon-icon {
  display: none;
}

.light-theme .sun-icon {
  display: none;
}

.light-theme .moon-icon {
  display: block;
}
/* Header JavaScript Styles */
.header.activated {
  box-shadow: 0 1px 0.5rem var(--transparent-light-color);
}

.menu.activated {
  box-shadow: 1px 1px 1rem var(--transparent-light-color);
  opacity: 1;
  transform: scale(1);
}

.menu-toggle-icon.activated .open-menu-icon {
  display: none;
}

.menu-toggle-icon.activated .close-menu-icon {
  display: block;
}
</style>
