<template>
  <div class="">
    <main-section />
    <div class="container">
      <advantages-section />
      <rules-section />
      <cards-section />
    </div>
    <footer-section />
  </div>
</template>

<script>
import AdvantagesSection from '../components/advantagesSection'
import CardsSection from '../components/cardsSection'
import FooterSection from '../components/footerSection'
import MainSection from '../components/mainSection'
import RulesSection from '../components/rulesSection'
export default {
  components: {
    MainSection,
    AdvantagesSection,
    RulesSection,
    CardsSection,
    FooterSection,
  },
}
</script>

<style lang="scss"></style>
