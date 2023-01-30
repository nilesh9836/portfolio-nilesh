<template>
  <div>
    <div v-for="project in projects" :key="project.id">
      <h2>{{ project.name }}</h2>
      <img :src="project.image" :alt="project.name" />
      <p>{{ project.description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          id: 1,
          name: "Project 1",
          image: "path/to/project1.jpg",
          description: "A description of project 1.",
        },
        {
          id: 2,
          name: "Project 2",
          image: "path/to/project2.jpg",
          description: "A description of project 2.",
        },
        {
          id: 3,
          name: "Project 3",
          image: "path/to/project3.jpg",
          description: "A description of project 3.",
        },
      ],
    };
  },
};
</script>
