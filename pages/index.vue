<template>
  <Gen
    ><h3 class="text-h4 mb-4 mt-5">Mathlab and Computing</h3>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo incidunt
      dicta porro nostrum mollitia aut aliquid fugiat! Dolorem natus, cum
      labore, iusto deserunt quod deleniti magni animi quasi reiciendis error.
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
