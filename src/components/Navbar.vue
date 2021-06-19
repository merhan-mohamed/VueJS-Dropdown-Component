<template lang="html">
  <nav>
    <div class="menu-items"><a href="#">Home</a></div>
    <div class="menu-items"><a href="#">About</a></div>
    <dropdown title='services' :items='services'/>
    <div class="menu-items"><a href="#">Contact</a></div>
  </nav>
</template>

<script>
import dropdown from "./dropdown.vue";
export default {
  name: "navbar",
  components: {
    dropdown,
  },
  data: () => ({
    services: [
      {
        title: "Web",
        link: "#",
      },
      {
        title: "Design",
        link: "#",
      },
      {
        title: "Videos",
        link: "#",
      },
    ],
  }),
};
</script>

<style>
nav {
  display: flex;
  align-items: center;
  justify-content: center;
}
nav .menu-items.active,
nav .menu-items:hover {
  background-color: #444;
  border-bottom-color: #ff5858;
}
nav .menu-items {
  padding: 10px 20px;
  color: white;
  text-align: center;
  border-bottom: 3px solid transparent;
  position: relative;
}

nav .menu-items a {
  color: inherit;
  text-decoration: none;
}
</style>
