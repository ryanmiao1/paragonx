<template>
  <div>
    <v-container>
      <h2 class="text-md-h2 text-h3 text-center">
        ParagonX Academy courses
      </h2>
      <div style="width: 80px; height: 4px" class="my-4 secondary mx-auto" />
      <div class="text--lighten-2 mt-4 text-body-1 text-center">
        Click on cards to see details and registration information.
        <p>The zoom link for all courses is <a href="https://us05web.zoom.us/j/7381417433?pwd=HE0Psmp89KYbnlFP4VYsc6KeQ2NELf.1">https://us05web.zoom.us/j/7381417433?pwd=HE0Psmp89KYbnlFP4VYsc6KeQ2NELf.1</a>.</p>
      </div>
    </v-container>
    <v-container v-if="onlineClasses.length>0" class="mt-2">
      <v-row class="mb-n8">
        <v-col cols="9">
          <h4 class="text-h4 text-left">
            Online Classes
          </h4>
        </v-col>
        <v-col><v-select v-model="currentSeason" class="mt-n1" outlined :items="seasons" /></v-col>
      </v-row>
      <v-row>
        <v-col
          v-for="(event,index) in onlineClasses"
          :key="index"
          cols="12"
          md="6"
        >
          <event-card
            :event="
              event"
          />
        </v-col>
      </v-row>
    </v-container>
    <v-container v-if="inPersonClasses.length>0" class="mt-2">
      <h4 class="text-h4 text-left">
        In-Person Classes
      </h4>
      <v-row class="mt-2">
        <v-col
          v-for="(event,index) in inPersonClasses"
          :key="index"
          cols="12"
          md="6"
        >
          <event-card
            :event="
              event"
          />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: 'CoursesIndex',
  async asyncData ({ params, error, $content }) {
    const events = await $content('events').sortBy('dateStart', 'asc').fetch()
    return { events }
  },
  data () {
    return {
      seasons: ['Spring 2026', 'Fall 2025', 'Summer 2025', 'Spring 2025', 'Fall 2024', 'Summer 2024', 'Spring 2024', 'Fall 2023', 'Summer 2023', 'Spring 2023', 'Fall 2022', 'Fall 2021'],
      currentSeason: 'Spring 2026'
    }
  },
  head () {
    return {
      title: 'Courses',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'ParagonX Academy is a 501(c)(3) student-led non-profit organization that strives to provide high-quality, readily available STEM education to everyone in need through free curricula.'
        }
      ]
    }
  },
  computed: {
    onlineClasses () {
      return this.events.filter(event => event.type === 'Online Class' && event.open && event.season === this.currentSeason).concat(this.events.filter(event => event.type === 'Online Class' && !event.open && event.season === this.currentSeason))
    },
    inPersonClasses () {
      return this.events.filter(event => event.type === 'In-Person Class' && event.open && event.season === this.currentSeason).concat(this.events.filter(event => event.type === 'In-Person Class' && !event.open && event.season === this.currentSeason))
    }
  }
}
</script>
