<template>
  <div>
    <header>
      <nav>
        <router-link :to="{ name: 'Home' }">Home</router-link>
        <router-link :to="{ name: 'About' }">About</router-link>
        <router-link :to="{ name: 'Projects' }">Projects</router-link>
        <router-link :to="{ name: 'Contacts' }">Contact</router-link>
      </nav>
    </header>

    <main>
      <router-view />
    </main>

    <footer>
      Copyright © 2021 Portfolio Website
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App',
  created() {
    // Fetch data from an API or database here
    // this.projects = data;
  },
  data() {
    return {
      projects: [
        {
          id: 1,
          name: 'Project 1',
          image: 'path/to/project1.jpg',
          description: 'A description of project 1.',
          link: 'http://project1.com'
        },
        {
          id: 2,
          name: 'Project 2',
          image: 'path/to/project2.jpg',
          description: 'A description of project 2.',
          link: 'http://project2.com'
        },
        {
          id: 3,
          name: 'Project 3',
          image: 'path/to/project3.jpg',
          description: 'A description of project 3.',
          link: 'http://project3.com'
        }
      ]
    }
  }
}
</script>
