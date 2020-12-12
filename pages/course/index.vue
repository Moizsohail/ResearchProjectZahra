<template>
  <Gen
    ><h3 class="text-h4 mb-4 mt-5">Courses</h3>

    <Grid :tiles="courses"
  /></Gen>
</template>
<script>
import Gen from '~/components/Gen'
import Grid from '~/components/Grid'
export default {
  components: {
    Gen,
    Grid,
  },
  computed: {
    courses() {
      return this.$store.state.course.data
    },
  },
}
</script>
