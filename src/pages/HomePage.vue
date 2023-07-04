<template>
  <div class="container">
    <HeaderPage/>
    <div>
      <SectionOne/>
      <SectionTwo/>
      <PlanePage/>
      <LocalPage/>
      <EvaluatePage/>
      <RegisterPage/>
      <FooterPgae/>
    </div>
  </div>
</template>
<script>
import HeaderPage from "@/components/HeaderPage.vue";
import SectionOne from "@/components/SectionOne.vue";
import SectionTwo from "@/components/SectionTwo.vue";
import PlanePage from "@/components/PlanePage.vue";
import LocalPage from "@/components/LocalPage.vue";
import EvaluatePage from "@/components/EvaluatePage.vue";
import RegisterPage from "@/components/RegisterPage.vue";
import FooterPgae from "@/components/FooterPgae.vue";
export default {
  components:{
    FooterPgae,
    RegisterPage,
    EvaluatePage,
    LocalPage,
    HeaderPage,
    SectionOne,
    SectionTwo,
    PlanePage
  }
}
</script>
<style scoped lang="scss">
.container{
  margin: 0 auto;
  position: relative;
}
@media (max-width: 600px) {
  .container{
  }
}
</style>