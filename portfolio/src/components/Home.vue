<template>
  <div>
    <h1>Welcome to my portfolio!</h1>
    <p>My name is {{name}} and I'm a {{occupation}}</p>
    <h2>Recent Projects</h2>
    <ul>
      <li v-for="project in projects" :key="project.id">
        {{ project.title }}
      </li>
    </ul>
  </div>
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
