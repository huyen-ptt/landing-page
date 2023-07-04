<template>
  <div class="feature">
    <div class="wrapper-feature">
      <div class="item-feature-big">Want anything to be easy with <span>LaslesVPN</span></div>
      <div class="item-feature-small">Lorem ipsum dolor sit amet consectetur. Quis tortor gravida nibh arcu id purus ullamcorper. Vel vel erat semper augue.</div>
      <button class="btn-feature">Get started</button>
    </div>
    <div class="img-section-one">
      <img src="@/assets/imgs/img-section-1.png">
    </div>
  </div>
  <div class="local">
    <div class="item-local">
      <img src="@/assets/imgs/user.png"/>
      <div>
        <div class="total">90+</div>
        <div class="distribution">Users</div>
      </div>
    </div>
    <div class="item-local">
      <img src="@/assets/imgs/location.png"/>
      <div>
        <div class="total">30+</div>
        <div class="distribution">Locations</div>
      </div>
    </div>
    <div class="item-local">
      <img src="@/assets/imgs/hierarchy-square-2.png"/>
      <div>
        <div class="total">50+</div>
        <div class="distribution">Servers</div>
      </div>
    </div>
  </div>
</template>
<style scoped lang="scss">
.feature{
  display: flex;
  align-items: center;
  gap:18px;
  padding-bottom: 67px;
  max-width: 1200px;
  margin: 0 auto;
  .wrapper-feature{
    .item-feature-big{
      font-size: 50px;
      font-weight: 400;
      padding-bottom: 42px;
      span{
        font-weight: 600;
      }
    }
    .item-feature-small{
      color: #5A5A5A;
      font-size: 16px;
      font-weight: 400;
      padding-bottom: 58px;
    }
    .btn-feature{
      color: #FFF;
      font-size: 18px;
      font-weight: 600;
      border-radius: 20px;
      background: var(--red, #F53838);
      padding: 13px 32px;
      border: 0;
      &:hover{
        cursor: pointer;
        color: #2B2B2B;
        background: #FCAEAE;
        transition: 1s;
      }
    }
  }
}
.local{
  max-width: 1000px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  gap:190px;
  justify-content: center;
  border-radius: 20px;
  background: #FFF;
  box-shadow: 7px 13px 35px 0px rgba(0, 0, 0, 0.09);
  padding: 37px;
  .item-local{
    display: flex;
    align-items: center;
    gap:23px;
    .total{
      font-size: 20px;
      font-weight: 600;
      color: var(--gray, #2B2B2B);
    }
    .distribution{
      font-size: 15px;
      font-weight: 400;
      color: var(--very-gray, #646464);
    }
  }

}
@media (max-width: 600px) {
  .feature{
    display: flex;
    flex-direction: column;
    padding: 100px 19px;
    .wrapper-feature{
      order: 3;
      margin-bottom: 30px;
      .item-feature-big{
        font-size: 34px;
        padding-bottom: 17px;
      }
      .item-feature-small{
        font-size: 11px;
        padding-bottom: 33px;
      }
    }
    .img-section-one{
      order: 2;
      padding-bottom: 34px;
      img{
        width: 100%;
      }
    }
  }
  .local{
    gap:40px;
    margin: 0 19px;
    padding: 30px 25px;
    .item-local{
      gap:13px;
      .total{
        font-size: 14px;
      }
      .distribution{
        font-size: 10px;
      }
    }
  }
}


</style>