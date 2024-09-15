<template>
  <li :class="classs">
    <a href="#" class="list-link">{{ item }}</a>
  </li>
</template>

<script>
export default {
  props: ['classs', 'item']
}
</script>
