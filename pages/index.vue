<template>
  <div>
    <v-container class="text-center">
      <h1 class="text-md-h1 text-h3  mt-md-6">
        Bringing <span class="primary--text">STEM Education</span> to Our Community
      </h1>
      <div class="text--lighten-2 mt-4 text-body-1">
        With nationally acclaimed instructors including USACO Finalists, MOP invitees, and Science Bowl winners, ParagonX Academy is a 501(c)(3) student-led non-profit organization that strives to provide readily available STEM education through free curricula.
      </div>
      <div class="mt-6">
        <v-btn x-large depressed to="/events" color="primary" class="my-1 mr-sm-1 w-full w-sm-auto">
          Spring 2026 Courses
        </v-btn>
        <v-btn x-large outlined href="https://discord.com/invite/kSXnnMm244" target="_blank" class="my-1 ml-sm-1 w-full w-sm-auto">
          Join Discord
        </v-btn>
      </div>
    </v-container>

    <v-container class="mt-6">
      <v-row>
        <v-col
          v-for="(item, i) in features"
          :key="i"
          cols="12"
          md="4"
        >
          <v-card class="py-4 px-2">
            <v-responsive max-width="300" class="mx-auto text-center">
              <div class="mb-2">
                <v-icon class="text-h1" color="primary">
                  {{ item.icon }}
                </v-icon>
              </div>
              <div class="text-h5 mt-3">
                {{ item.title }}
              </div>
              <div class="mt-2 text-body-2">
                {{ item.description }}
              </div>
            </v-responsive>
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <v-container class="mt-4">
      <h3 class="text-md-h3 text-h4 text-center">
        Features of our classes
      </h3>
      <div class="mt-6">
        <div
          v-for="(item, i) in courseFeatures"
          :key="i"
          class="mt-4"
        >
          <v-card class="py-4 px-2">
            <div class="d-flex">
              <div class="mr-2">
                <v-sheet
                  color="primary"
                  rounded
                  class="pa-2"
                  style="margin-top: 3px"
                  dark
                >
                  <v-icon>{{ item.icon }}</v-icon>
                </v-sheet>
              </div>
              <div>
                <div class="text-h5 font-weight-bold">
                  {{ item.title }}
                </div>
                <div class="text-body-2 mt-1">
                  {{ item.description }}
                </div>
              </div>
            </div>
          </v-card>
        </div>
      </div>
    </v-container>

    <v-container class="mt-4">
      <h3 class="text-md-h3 text-h4 text-center">
        Impact and statistics
      </h3>

      <v-carousel
        class="mt-4"
        cycle
        height="550"
        show-arrows-on-hover
      >
        <v-carousel-item
          v-for="(slide, i) in slides"
          :key="i"
        >
          <v-img :src="slide.image">
            <v-sheet>
              <div class="pa-1 text-body-1">
                {{ slide.caption }}
              </div>
            </v-sheet>
          </v-img>
        </v-carousel-item>
      </v-carousel>
      <v-row class="mt-2">
        <v-col
          v-for="(item, i) in stats"
          :key="i"
          cols="12"
          md="4"
        >
          <v-card class="pa-4">
            <div class="text-h2 text-lg-h1">
              {{ item.value }}
            </div>
            <div class="text-h6 text-lg-h5">
              {{ item.title }}
            </div>
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <v-container class="mt-4">
      <h3 class="text-md-h3 text-h4 text-center">
        Feedback from our students
      </h3>

      <v-row class="mt-6">
        <v-col
          v-for="(item, i) in testimonials"
          :key="i"
          cols="12"
          md="4"
        >
          <v-card class="pa-3 d-flex">
            <div class="text-h1 mr-2">
              “
            </div>
            <div class="text-body-2">
              {{ item.testimonial }}
            </div>
          </v-card>
          <div class="text-h7 mt-2 ml-1">
            {{ item.name }}
          </div>
        </v-col>
      </v-row>
    </v-container>
    <v-container class="mt-4">
      <h3 class="text-md-h3 text-h4 text-center">
        Partners
      </h3>

      <v-row class="mt-4">
        <v-col
          v-for="(item, i) in partners"
          :key="i"
          class="justify-center d-flex"
        >
          <a :href="item.link">
            <v-avatar size="150">
              <v-img :src="item.image" />
            </v-avatar>
          </a>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data () {
    return {
      features: [{
        icon: 'mdi-cast-education',
        title: 'Online Classes',
        description: 'We teach online courses on topics such as math, computer science, physics, chemistry, and more! By providing online education, we hope that people from around the world can easily access our classes for free.'
      }, {
        icon: 'mdi-bookmark-box-multiple',
        title: 'Teaching at the Library',
        description: 'We also teach classes in local libraries, with the goal of directly impacting our community and establishing a personal relationship with our students. Direct communication with an instructor and small class sizes make the learning process much easier.'
      }, {
        icon: 'mdi-account-voice',
        title: 'Speaker Events',
        description: 'We invite industry professionals, professors, and national science competition winners to share their knowledge and experience with our students.'
      }],
      courseFeatures: [{
        icon: 'mdi-medal',
        title: 'Award-Winning Instructors',
        description: 'Our instructors are some of the highest-ranking high school students in nationwide math and science competitions, guaranteeing that our course content is of the highest-quality.'
      }, {
        icon: 'mdi-message-text',
        title: 'Direct Communication',
        description: 'Throughout the week, students have the opportunity to directly communicate with our instructors and ask questions via our Discord server.'
      }, {
        icon: 'mdi-file-tree',
        title: 'Structured Curriculum and Homework',
        description: 'Our courses consist of eight classes, and the curriculum spanning these classes have been carefully cultivated by our instructors to maximize the usefulness and quality of knowledge that students will gain. Homework will also be assigned after each class. '
      }],
      testimonials: [{
        name: 'AMC 8 Student',
        testimonial: 'Alex was very knowledgeable and nice to speak with. He is a better teacher than many teachers that I have had in school, as he has personal experience with what he teaches.'
      }, {
        name: 'AMC 10 to AIME Student',
        testimonial: 'This course is really good! I learned quite a lot about AMC 10 concepts (specifically geometry and combinatorics). Austin and Neil are wonderful teachers who made the concepts very clear and gave motivated solutions to the problems.'
      }, {
        name: 'Biology and USABO Student',
        testimonial: 'Arjun was a very good instructor. He explained the concepts in an easy to understand way and clearly had lots of knowledge on the subject.'
      }],
      colors: [
        'indigo',
        'warning',
        'pink darken-2',
        'red lighten-1',
        'deep-purple accent-4'
      ],
      slides: [
        {
          image: '/images/carousel/2025-1.webp',
          caption: 'Karthik Veeramallu and Harshil Nukala, AP Physics 1, Spring 2025'
        },
        {
          image: '/images/carousel/2025-2.webp',
          caption: 'Vaishnav Krishnan, USACO Bronze, Spring 2025'
        },
        {
          image: '/images/carousel/2025-3.webp',
          caption: 'Pascal Qin, F=ma, Spring 2025'
        },
        {
          image: '/images/carousel/2025-4.webp',
          caption: 'Yash Belani and Ryan Miao, USACO Silver, Spring 2025'
        },
        {
          image: '/images/carousel/2025-5.webp',
          caption: 'Lucas Wu, Electromagnetism, Spring 2025'
        },
        {
          image: '/images/carousel/2025-6.webp',
          caption: 'Terry Xie, Introduction to USABO, Spring 2025'
        },
        {
          image: '/images/carousel/2025-7.webp',
          caption: 'Anushka Polapally, AMC 8, Spring 2025'
        },
        {
          image: '/images/carousel/2025-8.webp',
          caption: 'Kallie Wang and Arjun Joisha, AMC 10/12 to AIME, Spring 2025'
        },
        {
          image: '/images/carousel/2025-9.png',
          caption: 'Aarush Vailaya, Graph Theory, Spring 2025'
        }
      ],
      stats: [{
        title: 'Students Impacted',
        value: '1500' // total value: 1485, summer 2024 (not including events or spring 2024)
      }, {
        title: 'Courses and Events',
        value: '36' // summer 2024
      }, {
        title: 'Classes Taught',
        value: '200+' // total value: 216, summer 2024
      }],
      partners: [
        {
          name: 'Olympiad Prep Hub',
          image: '/images/partners/olympiadprephub.png',
          link: 'https://olympiadprephub.com/'
        },
        {
          name: 'Mitosisphere',
          image: '/images/partners/mitosisphere.png',
          link: 'https://mitosisphere.org/'
        },
        {
          name: 'BioCataalysis',
          image: '/images/partners/biocataalysis.png',
          link: 'https://biocataalysis.org'
        }
      ]
    }
  },
  head () {
    return {
      title: 'Home',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'ParagonX Academy is a 501(c)(3) student-led non-profit organization that strives to provide high-quality, readily available STEM education to everyone in need through free curricula.'
        }
      ]
    }
  }
}
</script>
