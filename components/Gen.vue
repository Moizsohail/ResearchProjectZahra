<template>
  <div>
    <NavBar></NavBar>
    <v-container>
      <Carousel></Carousel>
      <v-row>
        <v-col cols="8">
          <slot></slot>
        </v-col>
        <v-col>
          <Contact></Contact>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
import NavBar from '~/components/NavBar'
import Carousel from '~/components/Carousel'
import Contact from '~/components/ContactCard'
export default {
  components: {
    NavBar,
    Carousel,
    Contact,
  },
}
</script>
