<template>
  <CTASection></CTASection>
</template>

<script>
import CTASection from './components/CTASection.vue'

export default {
  name: 'App',
  components: {
    CTASection
  }
}
</script>

<style>
@font-face {
  font-family: TT commons pro;
  src: url('~@/assets/fonts/TT Commons Pro Normal.otf');
}
body{
  font-family: "TT Commons Pro";
  padding: 48px 20px 64px;
  margin: 0;
}
@media (min-width: 768px) {
  body{
    padding: 32px 48px 60px;
  }
}
</style>
