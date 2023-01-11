<template>
  <section>
    <h2>About Me</h2>
    <div v-html="bio"></div>
    <div>
      <h3>Skills</h3>
      <ul>
        <li v-for="skill in skills" :key="skill.id">{{ skill.name }}</li>
      </ul>
    </div>
    <div>
      <h3>Education</h3>
      <ul>
        <li v-for="education in educations" :key="education.id">
          {{ education.degree }} from {{ education.school }} ({{ education.graduationYear }})
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: 'About',
  data() {
    return {
      bio: 'I am a full-stack developer with 5 years of experience in web development. I am skilled in HTML, CSS, JavaScript, and various JavaScript frameworks such as Vue.js and React. I have experience working with various types of databases and I am always eager to learn new technologies.',
      skills: [
        { id: 1, name: 'JavaScript' },
        { id: 2, name: 'Vue.js' },
        { id: 3, name: 'React' },
        { id: 4, name: 'Node.js' },
        { id: 5, name: 'MongoDB' }
      ],
      educations: [
        {
          id: 1,
          degree: 'BSc in Computer Science',
          school: 'University of XYZ',
          graduationYear: '2015'
        },
        {
          id: 2,
          degree: 'MSc in Web Development',
          school: 'University of ABC',
        }],
    }
  }
}
  </script>
