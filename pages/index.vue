<template>
  <div class="">
    <main-section />
    <div class="container">
      <advantages-section />
    </div>
    <rules-section />
    <div class="container">
      <flex-section />
    </div>
    <cards-section />
    <banner-section />
    <footer-section />
  </div>
</template>

<script>
import AdvantagesSection from '../components/advantagesSection'
import BannerSection from '../components/bannerSection'
import CardsSection from '../components/cardsSection'
import FooterSection from '../components/footerSection'
import MainSection from '../components/mainSection'
import RulesSection from '../components/rulesSection'
import flexSection from '../components/flexSection'
export default {
  components: {
    MainSection,
    AdvantagesSection,
    RulesSection,
    CardsSection,
    FooterSection,
    BannerSection,
    flexSection,
  },
}
</script>

BannerSection
<style lang="scss"></style>
