<template>
    <header class="header">
      <div class="header__wrapper">
        <div class="header__btn">
          <div class="header__span-wrapper">
            <span class="header__span span1"></span>
            <span class="header__span span2"></span>
            <span class="header__span span3"></span>
        </div>
        </div>
        <div class="header__wrapper-container container">
        <div class="header__logo">
          <img src="../assets/img/logo.svg" alt="">
        </div>
        <div class="header__form-wrapper">
        <form action="header__form" class="header__form">
          <button  class="header__form-buttom">All <img src="../assets/img/arrow.svg" alt=""></button>
          <div class="line"></div>
          <input type="text" name="header__form" id="" class="header__input" placeholder="Search Mobiles, TV, Laptops,Tablets, Beauty & Personal Care etc.">
          <img class="header__search" src="../assets/img/search.svg" alt="">
        </form>
        </div>
        <div class="header__login">
          <div class="header__login-mark">
            <img v-on:click="console" src="../assets/img/mark.svg" alt="">
          </div>
          <div class="header__login-shop">
            <img src="../assets/img/shop.svg" alt="">
          </div>
          <div class="line"></div>
          <div class="header__login-location">
            <img src="../assets/img/location.svg" alt="">
            <p>Pacistan</p>
          </div>
          <div class="header__login-login">
            <a href="#">Login</a>
          </div>
        </div>
        </div>
      </div>
    </header>
</template>

<script>
export default {
  name: 'Header',
  methods: {
    console: function() {
        console.log('Привет');
        
      }
    
  }
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" >
  .header {
    &__wrapper {
      display: flex;
      align-items: center;
      justify-content: space-between;
      // position: relative;
      // padding-top: 30px ;
    }
    &__wrapper-container {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    &__btn {
      cursor: pointer;
      width: 132px;
      height: 108px;
      max-width: 100%;
      display: block;
      background-color: $primary;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
    }
    &__input {
      border: none;
      width: 442px;
      max-width: 100%;
      font-size: 14px;
      background: none;
      color: #232F3E;
    }
    &__form {
      max-width: 100%;
    }
    &__form-wrapper {
      background-color: #F2F2F2;
      padding: 17px;
      width: 600px;
      max-width: 100%;
      margin-left: 47px;
      position: relative;
      margin-right: 68px;
    }

    &__login {
      display: flex;
    }
  }
  .header__search {
    right: 24px;
    position: absolute;
    cursor: pointer;
  }
  .header__form {
    display: flex;
    align-items: center;
  }
  .header__form-buttom img {
    margin: 0 13px 0 12px;
    } 
    
  .header__form-buttom {
    background: none;
    border: none;
    font-size: 12px;
    font-weight: Regular;
  }
  .header__span-wrapper {
    top: 50%;
    left: 50%;
    transform: translateY(-50%);
  }
  .header__span {
    display: block;
    width: 26px;
    height: 2px;
    background-color: #fff;
    &:not(:last-child) {
      margin-bottom: 5px;
    }
  }

  .span1 {
    width: 18px;
  }
  .span3 {
    width: 13px;
  }
  
  .header__login {
    display: flex;
    align-items: center;
  }
  .header__login-mark{
    cursor: pointer;
    margin-right: 33px;
  }
  .header__login-shop{
    cursor: pointer;
    margin-right: 23px;
  }
  .line {
    display: block;
    width: 32px;
    height: 1px;
    background-color: #232F3E;
    transform: rotate(90deg);
    opacity: 16%;
  }
  .header__login-location {
    display: flex;
    align-items: center;
    margin-right: 24px;
    cursor: pointer;
  }

  .header__login-login {
    cursor: pointer;
    padding: 12px 32px;
    background-color: $primary;
    transition: all .3s;
  }
  .header__login-login a {
    color: #fff;
    text-decoration: none;
    font-weight: 400;
    font-size: 12px;
  }
  .header__login-login:hover {
    background-color: #48515a;
  }


  </style>
