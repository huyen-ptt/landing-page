<template>
  <div class="header">
    <div class="header-left">
      <img src="@/assets/imgs/logo.png"/>
      <div>Lasles<span>VPN</span></div>
    </div>
    <div class="wrapper-menu">
      <a class="item-menu">features</a>
      <a class="item-menu">Pricing</a>
      <a class="item-menu">Testimonial</a>
      <a class="item-menu">Help</a>
    </div>
    <div class="btn-sign-in">
      <button class="sign-in">Sign in</button>
      <button class="sign-up">Sign up</button>
    </div>
    <i class="fa-solid fa-bars"></i>
  </div>
</template>
<style scoped lang="scss">
.header{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 30px;
  padding-bottom: 130px;
  max-width: 1200px;
  margin: 0 auto;
  .header-left{
    display: flex;
    gap:3px;
    align-items: center;
    font-weight: 400;
    color: #151515;
    font-size: 18px;
    cursor: pointer;
    span{
      font-weight: 600;
    }
  }
  .fa-bars{
    display: none;
  }
  .wrapper-menu{
    display: flex;
    gap:56px;
    align-items: center;
    .item-menu{
      color: var(--gray, #2B2B2B);
      font-size: 16px;
      font-weight: 400;
      cursor: pointer;
    }
  }
  .btn-sign-in{
    display: flex;
    gap:15px;
    align-items: center;
    .sign-in{
      font-size: 16px;
      font-weight: 400;
      padding:8px 15px;
      border-radius: 20px;
      border: 1px solid rgba(0, 0, 0, 0.00);
      background: white;
      &:hover{
        cursor: pointer;
        background: lightgoldenrodyellow;
      }
    }
    .sign-up{
      font-size: 16px;
      font-weight: 400;
      padding:8px 15px;
      border-radius: 20px;
      border: 2px solid var(--red, #F53838);
      background: white;
      &:hover{
        cursor: pointer;
        background: lightgoldenrodyellow;
      }
    }
  }
}
@media (max-width: 450px) {
  .header{
    padding: 15px 19px 24px 19px;
    .wrapper-menu{
      display: none;
    }
    .btn-sign-in{
      display: none;
    }
    .fa-bars{
      display: block;
      font-size: 24px;
    }
  }
}
</style>