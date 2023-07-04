<template>
  <div :class="getClass()">
      <span>
        <i @click="closeMenu" class="fa-solid fa-xmark"></i>
      </span>
    <ul>
      <li v-for="m in menu " :key="m.url">
        <a :href="m.url" @click="toggleMenu">{{m.name}}</a>
      </li>
    </ul>
  </div>
  <div class="header">
    <div class="header-left">
      <img src="@/assets/imgs/logo.png"/>
      <div>Lasles<span>VPN</span></div>
    </div>
    <div class="wrapper-menu">
      <a class="item-menu" href="#features">Features</a>
      <a class="item-menu" href="#pricing">Pricing</a>
      <a class="item-menu" href="#testimonial">Testimonial</a>
      <a class="item-menu" href="#help">Help</a>
    </div>
    <div class="btn-sign-in">
      <button class="sign-in">Sign in</button>
      <button class="sign-up">Sign up</button>
    </div>
    <i @click="openMenu=!openMenu" class="fa-solid fa-bars"></i>
  </div>

</template>
<script>
export default {
  data() {
    return {
      openMenu: false,
      menu: [
        {url:"#features",name:"Features"},
        {url:"#pricing",name:"Pricing"},
        {url:"#testimonial",name:"Testimonial"},
        {url:"#help",name:"Help"},
      ]
    }
  },
  methods:{
    closeMenu(){
      this.openMenu = false
    },
    toggleMenu(){
      this.openMenu = !this.openMenu
    },
    getClass(){
      if(this.openMenu){
        return 'mobile-link open-menu'
      }else {
        return 'mobile-link close-menu'
      }
    },
  }
}
</script>
<style scoped lang="scss">
.header{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 30px;
  padding-bottom: 130px;
  max-width: 1200px;
  margin: 0 auto;
  .mobile-link{
    display: none;
  }
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
        background: #FCAEAE;
        transition: 1s;
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
        background:#FCAEAE;
        transition: 1s;
      }
    }
  }
}
@media (max-width: 450px) {
  .mobile-link {
    align-items: center;
    background-color: #fff;
    display: flex;
    height: 100vh;
    justify-content: center;
    left: 0;
    position: fixed;
    text-align: center;
    top: 0;
    transition: all .3s ease-in-out;
    width: 100%;
    z-index: 300;
    .fa-solid{
      font-size: 30px;
    }
    span{
      cursor: pointer;
      font-size: 3.3rem;
      position: absolute;
      right: 4rem;
      top: 2rem;
    }
    ul{
      display: flex;
      flex-direction: column;
      font-size: 2rem;
      gap: 4rem;
      list-style: none;
      a{
        color: #000;
        font-weight: 500;
        text-decoration: none;
      }
    }
  }
  .open-menu {
    left: 0;
  }
  .close-menu {
    left: -100%;
  }
  .header {
    align-items: center;
    background-color: #fff;
    box-shadow: 0 0 10px rgba(0, 0, 0, .09);
    display: flex;
    font-size: 1.7rem;
    height: auto;
    justify-content: space-between;
    left: 0;
    padding: 25px 40px 25px 50px;
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 3;

    .wrapper-menu {
      display: none;
    }

    .btn-sign-in {
      display: none;
    }

    .fa-bars {
      display: block;
      font-size: 24px;
    }
  }
}
</style>