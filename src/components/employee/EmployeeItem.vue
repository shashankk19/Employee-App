<template>
  <li>
    <base-card>
      <header>
        <h3>{{ name }}</h3>
        <p>{{ title }}</p>
        <base-button mode="flat">Delete</base-button>
      </header>
      <nav>
        <a :href="link">Reach out</a>
      </nav>
    </base-card>
  </li>
</template>

<script>
import BaseButton from '../UI/BaseButton.vue';

export default {
  props: ['name', 'title', 'link'],
  components: {
    BaseButton,
  },
  data() {},
};
</script>

<style scoped>
li {
  margin: auto;
  max-width: 40rem;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

h3 {
  font-size: 1.25rem;
  margin: 0.5rem 0;
}

p {
  margin: 0.5rem 0;
}

a {
  text-decoration: none;
  color: #ce5c00;
}

a:hover,
a:active {
  color: #c89300;
}
</style>
