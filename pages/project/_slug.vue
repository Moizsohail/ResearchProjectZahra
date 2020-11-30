<template>
  <div>
    <Gen>
      <nuxt-content :document="doc" />
    </Gen>
  </div>
</template>

<script>
import Gen from '~/components/Gen'
export default {
  async asyncData({ $content, params }) {
    const doc = await $content('/projects/' + (params.slug || 'index')).fetch()
    return { doc }
  },
  components: {
    Gen,
  },
}
</script>
