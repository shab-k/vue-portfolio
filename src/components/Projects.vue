<template>
  <section id="projects">
    <div class="container">
      <div class="content-bg">
        <h1 class="text-center">Projects</h1>
        <div class="card-container">
          <div class="card" v-for="project in projects" :key="project.id">
            <div class="grid-area card-image">
              <img :src="require('../assets/images/' + project.photo)" />
            </div>
            <div class="grid-area card-body">
              <h6 class="card-title text-center">{{ project.title }}</h6>
              <p class="card-text micro semi-bold">{{ project.description }}</p>
              <ul class="stack micro">
                <li v-for="(tech, index) in project.technologies" :key="index">
                  - <span class="chip">{{ tech }}</span>
                </li>
              </ul>
              <br />
              <br />
            </div>
            <div class="grid-area card-action" v-if="project.id == 7">
              <a
                type="button"
                class="disabled button-link"
                data-toggle="tooltip"
                data-placement="bottom"
                title="shab.k.web [at] gmail"
                >DB Files</a
              >
              <a :href="project.github" class="button-link" target="_blank"
                >Github</a
              >
            </div>
            <div v-else class="grid-area card-action">
              <a :href="project.url" class="button-link" target="_blank"
                >Live</a
              >
              <a :href="project.github" class="button-link" target="_blank"
                >Github</a
              >
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Projects',
  data () {
    return {
      projects: [
        {
          id: '9',
          title: 'Wexperts React',
          description: 'A react project with full CRUD functionality',
          technologies: ['React', 'Redux', 'Styled components', 'Firebase'],
          photo: 'wexperts-react-fb-shot.jpg',
          url: 'https://wexperts-react.web.app/',
          github: 'https://github.com/shab-k/wexperts-react-fb'
        },
        {
          id: '8',
          title: 'Vue Portfolio',
          description: 'I rebuilt & redesigned my portfolio website using:',
          technologies: ['Vue', 'BEM', 'Sass', 'Flex', 'Netlify', 'CSS Grids'],
          photo: 'portfolio-screenshot.jpg',
          url: 'https://adoring-northcutt-103687.netlify.app',
          github: 'https://github.com/shab-k/vue-portfolio'
        },
        {
          id: '7',
          title: 'Resume Builder',
          description: 'A full stack CRUD app built with:',
          technologies: ['HTML5', 'Sass', 'CSS Grids', 'Flex', 'PHP', 'My SQL'],
          photo: 'resume-builder-screenshot.jpg',
          url: '#',
          github: 'https://github.com/shab-k/resume_builder'
        },
        {
          id: '6',
          title: 'Wexperts',
          description:
            'A landing page which is partially accessible, built with:',
          technologies: ['HTML5', 'Sass(+Flexbox + BEM + OOCSS)', 'Netlify'],
          photo: 'wexperts_screenshot.jpg',
          url: 'https://blissful-clarke-d16757.netlify.com/',
          github: 'https://github.com/shab-k/wexperts'
        },
        {
          id: '5',
          title: 'Bibliophile',
          description: 'A React app built with:',
          technologies: [
            'React',
            'Redux',
            'Materialize CSS',
            'Moment.js',
            'NYTimes Book API',
            'Firebase(Hosting+DB)'
          ],
          photo: 'bibliophile-screenshot.jpg',
          url: 'https://bibliophile-8ffc8.firebaseapp.com/',
          github: 'https://github.com/shab-k/bibliophile'
        },
        {
          id: '4',
          title: 'Blogit',
          description: 'A CMS app for managing blogs built with:',
          technologies: ['Vue', 'Materialize CSS', 'Firebase(DB, Hosting)'],
          photo: 'blogit_screenshot.jpg',
          url: 'https://blogit-69789.firebaseapp.com/',
          github: 'https://github.com/shab-k/blogit'
        },
        {
          id: '3',
          title: 'My Portfolio',
          description: 'My potfolio website built with:',
          technologies: ['HTML5', 'Bootstrap'],
          photo: 'portfolio-screenshot.jpg',
          url: 'https://shabnam-k.me/',
          github: 'https://github.com/shab-k/myportfolio'
        },
        {
          id: '2',
          title: 'Vuepress Blog',
          description: 'A Vuepress blog built with:',
          technologies: ['Vue.js', 'Vuepress', 'Materialize CSS'],
          photo: 'vuepress-screenshot.jpg',
          url: 'https://shab-k.github.io/myvuepress/blog/',
          github: 'https://github.com/shab-k/myvuepress'
        },
        {
          id: '1',
          title: 'Personal Website',
          description: 'A personal website built with:',
          technologies: ['HTML5', 'Javascript', 'Materialize CSS'],
          photo: 'personal_site_screenshot.jpg',
          url: 'https://shabnam-k.me/materialize-project/index.html',
          github:
            'https://github.com/shab-k/myportfolio/tree/master/dist/materialize-project'
        }
      ]
    }
  }
}
</script>
