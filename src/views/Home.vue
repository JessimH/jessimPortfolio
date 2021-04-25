<template>
  <div class="home">
    <InfoCard />
    <Presentation />
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import InfoCard from '@/components/InfoCard.vue'
import Presentation from '../components/Presentation.vue'
import Footer from '../components/Footer.vue'

export default {
  name: 'Home',
  components: {
    InfoCard,
    Presentation,
    Footer
  }
}
</script>
