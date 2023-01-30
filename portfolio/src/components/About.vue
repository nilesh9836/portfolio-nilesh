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
          {{ education.degree }} from {{ education.school }} ({{
            education.passingYear
          }})
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "About",
  data() {
    return {
      bio: "I am a front-end developer with 4 years of experience in web development. I am skilled in HTML, CSS, JavaScript, and various JavaScript frameworks such as Vue.js and React. I have experience working with various types of databases and I am always eager to learn new technologies.",
      skills: [
        { id: 1, name: "JavaScript" },
        { id: 2, name: "HTML5" },
        { id: 3, name: "CSS3" },
        { id: 4, name: "Vue.js" },
        { id: 5, name: "Java" },
        { id: 5, name: "Data Structure & Algorithm" },
      ],
      educations: [
        {
          id: 1,
          degree: "B.Tech in Computer Science & Engineering (8.11 DGPA)",
          school: "Institute of Engineering & Management",
          passingYear: "2019",
        },
        {
          id: 2,
          degree: "High School (80%)",
          school: "Don Bosco Convent School",
          passingYear: "2014",
        },
        {
          id: 2,
          degree: "10th (10 CGPA)",
          school: "Jawahar Navodaya vidyalaya",
          passingYear: "2012",
        },
      ],
    };
  },
};
</script>
