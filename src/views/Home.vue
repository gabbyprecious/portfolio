<template>
  <div class="home">
    <Name />
    <Skills />
  </div>
</template>

<script>
import Name from '@/components/Name.vue'
import Skills from '@/components/Skills.vue'
export default {
  name: 'Home',
  components: {
    Name,
    Skills
  }
}
</script>
