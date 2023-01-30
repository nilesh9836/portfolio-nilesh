<template>
  <v-container>
     <h1>Welcome </h1>
     <p>My name </p>
  </v-container>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      name: "John Doe",
      occupation: "Web Developer",
      projects: [
        { id: 1, title: "Project A" },
        { id: 2, title: "Project B" },
        { id: 3, title: "Project C" },
      ],
    };
  },
};
</script>
