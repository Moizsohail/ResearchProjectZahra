<template>
  <Gen
    ><h3 class="text-h4 mb-4 mt-5">Mathlab and Computing</h3>
    <p>
      My goal is to further develop mathematics as a key technology, give
      innovative impetus and implement it in practice together with industry
      partners. Methodologically, the research areas focus on modeling,
      simulation and optimization. Integral parts of the projects are consulting
      and implementation, support in the application of high-performance
      computing and providing tailor-made software solutions. I develop
      simulation software along with using existing ones, often in cooperation
      with leading software companies. Nowadays, companies of all sizes use
      simulations on regular bases which gives them benefit in terms of product
      innovation and quality assurance. My clients and users are mainly in the
      automotive, textile, finance and environmental enginnering
    </p>
    <Grid :tiles="fields"
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
    fields() {
      return this.$store.state.data
    },
  },
}
</script>
