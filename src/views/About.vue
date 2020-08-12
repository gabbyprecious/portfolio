<template>
  <div class="about">
    <Name />
    <Skills />
  </div>
</template>

<script>
import Name from '@/components/Name.vue'
import Skills from '@/components/Skills.vue'
export default {
  name: 'About',
  components: {
    Name,
    Skills
  }
}
</script>
