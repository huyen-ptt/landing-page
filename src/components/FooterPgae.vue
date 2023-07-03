<template>
  <div class="footer">
    <div class="title">
      <div class="logo">
        <img src="@/assets/imgs/logo.png"/>
        <div>Lasles<span>VPN</span></div>
      </div>
      <div class="title-footer-small">Lorem ipsum dolor sit amet consectetur. Quis<br> tortor gravida nibh arcu id purus ullamcorper.<br> Vel vel erat semper augue.</div>
      <div class="wrapper-contact">
        <div class="item-contact">
          <i class="fa-brands fa-facebook"></i>
        </div>
        <div class="item-contact">
          <i class="fa-solid fa-phone"></i>
        </div>
        <div class="item-contact">
          <i class="fa-brands fa-youtube"></i>
        </div>
      </div>
    </div>
    <div class="bao-wrapper">
      <div class="wrapper-item">
        <div class="item-active">Product</div>
        <div class="item">Download</div>
        <div class="item">Pricing</div>
        <div class="item">Locations</div>
        <div class="item">Server</div>
        <div class="item">Countries</div>
        <div class="item">Blog</div>
      </div>
      <div class="wrapper-item">
        <div class="item-active">Engage</div>
        <div class="item">LaslesVPN?</div>
        <div class="item">FAQ</div>
        <div class="item">Tutorials</div>
        <div class="item">About us</div>
        <div class="item">Privacy policy</div>
        <div class="item">Terms of service</div>
      </div>
      <div class="wrapper-item">
        <div class="item-active">Earn money</div>
        <div class="item">Become partner?</div>
        <div class="item">Affilite</div>
      </div>
    </div>
  </div>
</template>
<style scoped lang="scss">
.footer{
  display: flex;
  align-items: center;
  justify-content: center;
  background: #F4F4F4;
  gap:155px;
  padding: 40px 0 60px 0;
  margin: 0 auto;
  .logo{
    display: flex;
    align-items: center;
    gap:11px;
    color: #151515;
    font-size: 18px;
    font-weight: 400;
    padding-bottom: 23px;
    span{
      font-weight: 500;
    }
  }
  .title-footer-small{
    color: #5A5A5A;
    font-size: 15px;
    font-weight: 400;
    padding-bottom: 20px;
  }
  .wrapper-contact{
    display: flex;
    align-items: center;
    gap:26px;
    .item-contact{
      border-radius: 999px;
      background: var(--red-2, rgba(245, 56, 56, 0.10));
      width: 37px;
      height: 37px;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      i{
        font-size: 18px;
        color: #F53838;
        padding: 3px;
      }
    }
  }
  .bao-wrapper{
    display: flex;
    gap:93px;
    .item-active{
      color: var(--normal, #151515);
      font-size: 16px;
      font-weight: 600;
      padding-bottom: 18px;
    }
    .item{
      color: var(--very-gray, #646464);
      font-size: 15px;
      font-weight: 400;
      padding-bottom: 18px;
    }
  }
}
@media (max-width: 450px) {
  .footer{
    display: flex;
    flex-direction: column;
    padding: 40px 19px;
    gap:50px;
    .title{
      order: 1;
      display: flex;
      justify-content: center;
      flex-direction: column;
      align-items: center;
      .title-footer-small{
        text-align: center;
      }
    }
  }
}
</style>