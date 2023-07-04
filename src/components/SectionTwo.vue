<template>
  <div class="setion-two" id="features">
    <img class="logo-section-two" src="@/assets/imgs/img-section-2.png"/>
    <div>
      <div class="many-features">We provide many features you can use</div>
      <div class="title-small">Lorem ipsum dolor sit amet consectetur. Quis tortor gravida nibh arcu id purus ullamcorper. Vel vel erat semper augue.</div>
      <div class="wrapper-featuress">
        <div class="item-featuress">
          <img src="@/assets/imgs/tick-circle.png"/>
          <div>Powerfull online protection.</div>
        </div>
        <div class="item-featuress">
          <img src="@/assets/imgs/tick-circle.png"/>
          <div>Internet with borders</div>
        </div>
        <div class="item-featuress">
          <img src="@/assets/imgs/tick-circle.png"/>
          <div>Supercharged VPN</div>
        </div>
        <div class="item-featuress">
          <img src="@/assets/imgs/tick-circle.png"/>
          <div>No specific time limits</div>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped lang="scss">
.setion-two{
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap:182px;
  padding-top: 60px;
  padding-bottom: 75px;
  max-width: 1200px;;
  margin: 0 auto;
  .many-features{
    color: var(--gray, #2B2B2B);
    font-size: 30px;
    font-weight: 600;
    padding-bottom: 10px;
  }
  .title-small{
    color: #5A5A5A;
    font-size: 16px;
    font-weight: 400;
    padding-bottom: 13px;
  }
  .wrapper-featuress{
    .item-featuress{
      display: flex;
      align-items: center;
      padding-bottom: 26px;
      color: var(--gray, #2B2B2B);
      font-size: 16px;
      font-weight: 600;
      gap:10px;
    }
  }
}
@media (max-width: 450px) {
  .setion-two{
    display: block;
    padding: 30px 19px;
    .logo-section-two{
      width: 100%;
      padding-bottom: 28px;
    }
    .many-features{
      font-size: 20px;
      padding-bottom: 10px;
    }
    .title-small{
      font-size: 10px;
    }
    .wrapper-featuress{
      .item-featuress{
        padding: 0 19px 15px 19px;
        div{
          font-size: 11px;
        }

      }
    }
  }
}
</style>