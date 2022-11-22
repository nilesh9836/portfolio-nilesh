<template>
  <v-container fluid grid-list-md class="pa-0">
    <v-row
      class="pa-0 row-center pt-6"
      justify-content="center"
      style="background: #2b44ff"
    >
      <v-chip class="ma-2 pa-2 custom-chip" color="#ffff" text-color="primary">
        <v-btn-toggle v-model="text" color="accent-3" group text rounded>
          <v-btn value="about"> About me </v-btn>

          <v-btn value="myWork"> My work </v-btn>

          <v-btn rounded color="primary" dark value="contactMe">
            Contact me
          </v-btn>
        </v-btn-toggle>
      </v-chip>
    </v-row>
    <v-row class="pa-10">
      <v-col style="direction: rtl !important">
        <div style="color: blue" class="py-2"><h1>Let's Talk Business</h1></div>
        <div class="py-2">What Can I Do For You ?</div>
        <div class="py-2">
          With roughly 10 years experience in the tech industry, I can help you
          achieve your business
        </div>
        <div class="py-2">
          tech goals by implementing the correct solutions.
        </div>
      </v-col>
      <v-col>
        <ul>
          <li class="py-2">
            <span>Architecture Design and Implementation</span>
          </li>
          <li class="py-2"><span>Technical Advice</span></li>
          <li class="py-2"><span>Technical Consultant</span></li>
          <li class="py-2"><span>Open Source Collaboration</span></li>
        </ul>
      </v-col>
    </v-row>
    <v-row style="background: #93b6ed">
      <v-col> </v-col>
      <v-col>
        <div class="pb-3" style="font-family: sans-serif">
          <h2>About Me</h2>
        </div>
        <div>
          <pre style="font-family: sans-serif !important">{{
            `I’m Nilesh, I’m a frontend developer, 
 and I specialize in efficient Vue apps and CSS & HTML that just work across all platforms and browsers. 
 I care deeply about building interfaces that are usable and pleasant for the most number of people possible. 
 My professional life has been 100% driven by my passion for design and structure. 
 I was sketching crazy detailed 3d models for fun when I was a kid, 
 started building promo websites for small businesses while in college. 
 For three years, I have been working for a product based company where we develop a lot of functionality in my
 product which is helpful for our clients. Right now, I’m excited about the still very complicated WebAssembly, 
 and working towards becoming a Vue senior. In the following years, I also plan to explore the “server-side” more 
 and become a better-rounded full-stack dev.
           `
          }}</pre>
        </div>
        <div>
          <div class="pb-3" style="font-family: sans-serif">
            <h2>What I'm good at</h2>
          </div>
          <ul>
            <li>Bringing products to live</li>
            <li>Quirky designs</li>
            <li>Backend solutions</li>
            <li>Automation</li>
            <li>Putting personality into services</li>
            <li>PWAs (progressive web apps)</li>
            <li>Complete solutions, front to back</li>
            <li>Integrations</li>
            <li>Cloud platforms</li>
            <li>Internet Of Things</li>
            <li>Public Speaking</li>
            <li>Links</li>
            <li>Linkedin</li>
            <li>Colchester Digital</li>
            <li>Github</li>
            <li>Stackoverflow</li>
            <li>Codersrank</li>
            <li>Insta</li>
            <li>Facebook Page</li>
          </ul>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {};
</script>

<style scoped>
.custom-chip {
  height: 68px !important;
  border-radius: 50px !important;
  transform: translateY(42px) !important;
  box-shadow: 5px 10px #f4ecec;
}
.row-center {
  display: flex;
  justify-content: center;
}
</style>