<template>
  <div class="local">
    <div class="title-local">
      <div class="title-local-big">Huge global network<br> of fast VPN</div>
      <div class="title-local-small">
        Lorem ipsum dolor sit amet consectetur. Quis tortor gravida nibh arcu id<br> purus ullamcorper. Vel vel erat semper augue.
      </div>
    </div>
    <div>
      <img class="map" src="@/assets/imgs/local (2).png"/>
    </div>
  </div>
  <div class="bao-nhan-hieu">
    <img class="nhan-hieu" src="@/assets/imgs/sponsored.png"/>
  </div>
</template>
<style scoped lang="scss">
.local{
  padding-top: 90px;
  display: flex;
  align-items: center;
  flex-direction: column;
  max-width: 1200px;
  margin: 0 auto;
  .title-local{
    margin-bottom: 50px;
    .title-local-big{
      color: var(--gray, #2B2B2B);
      font-weight: 600;
      font-size: 25px;
      padding-bottom: 10px;
      text-align: center;
    }
    .title-local-small{
      text-align: center;
      color: #5A5A5A;
      font-weight: 400;
      font-size: 16px;
    }
  }
  .map{
    padding:0 20px;
    margin-bottom: 33px;
  }
}
.bao-nhan-hieu{
  display: flex;
  align-items: center;
  justify-content: center;
}
@media (max-width: 450px) {
  .local{
    padding: 0 19px;
    margin-top: 50px;
    .title-local{
      margin-bottom: 25px;
      .title-local-big{
        font-size: 18px;
        padding-bottom: 11px;
      }
      .title-local-small{
        font-size: 11px;
        padding-bottom: 25px;
      }
    }
    .map{
      width: 100%;
      margin-bottom: 38px;
    }
  }
  .bao-nhan-hieu{
    .nhan-hieu{
      width: 100%;
      padding: 0 19px;

    }
  }
}
</style>