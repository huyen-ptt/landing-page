<template>
  <div class="register" id="help">
    <div class="title-register">
      <div class="title-register-big">Subscribe now for<br>
        get special features!</div>
      <div class="title-register-small">Lorem ipsum dolor sit amet </div>
    </div>
    <button class="btn-register">Subscribe now</button>
  </div>
</template>
<style scoped lang="scss">
.register{
  //position: absolute;
  //bottom: 337px;
  //left: 146px;
  transform: translate(0%, 8%);
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1100px;
  margin: 0 auto;
  padding: 50px 56px;
  border-radius: 20px;
  background: #FFF;
  box-shadow: 12px 18px 54px 0px rgba(0, 0, 0, 0.11);

  .title-register{
    .title-register-big{
      color: var(--gray, #2B2B2B);
      font-size: 25px;
      font-weight: 600;
      padding-bottom: 17px;
    }
    .title-register-small{
      color: #5A5A5A;
      font-size: 16px;
      font-weight: 400;
      padding-bottom: 17px;
    }
  }
  .btn-register{
    border-radius: 20px;
    background: var(--red, #F53838);
    color: #FFF;
    font-size: 18px;
    font-weight: 600;
    padding: 15px 45px;
    border: 0;
    &:hover{
      cursor: pointer;
      color: #2B2B2B;
      background: #FCAEAE;
      transition: 1s;
    }
  }
}
@media (max-width: 450px) {
  .register{
    margin: 50px 19px;
    display: block;
    .title-register{
      .title-register-small{
        padding-bottom: 64px;
      }
    }
  }
}
</style>