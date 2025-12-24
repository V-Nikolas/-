<template>
  <div>
    <HeroSection />
    <section class="features container">
      <FeatureCard 
        v-for="i in 3" 
        :key="i" 
        :title="'Feature ' + i"
        :description="'Description for feature ' + i"
      />
    </section>
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection.vue'
import FeatureCard from '~/components/FeatureCard.vue'

export default {
  components: { HeroSection, FeatureCard }
}
</script>

<style scoped>
.features {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 20px;
  margin-top: 50px;
}
</style>