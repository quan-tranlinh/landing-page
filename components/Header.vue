<template>
  <div class="header">
    <div class="header-top">
      <h1 class="header-logo">
        <a href="/">
          <img src="/img/logo.png" alt="logo"/>
        </a>
      </h1>
      <nav class="header-nav">
        <NuxtLink to="/">About</NuxtLink>
        <NuxtLink to="/">Games</NuxtLink>
        <NuxtLink to="/">Partners</NuxtLink>
        <NuxtLink to="/">Contact us</NuxtLink>
        <div class="lang-select">
          <select class="form-control">
            <option value="usa">English</option>
            <option value="vn">Vietnamese</option>
          </select>
        </div>
      </nav>
    </div>
    <div class="banner">
      <h2 class="banner-title">We’re <br class="isSP">Getting Ready</h2>
      <div class="banner-time">
        <div class="banner-time-wrap">
          <span class="banner-time-wrap-number">30</span>
          <span class="banner-time-wrap-unit">days</span>
        </div>
        <span class="colon">:</span>
        <div class="banner-time-wrap">
          <span class="banner-time-wrap-number">18</span>
          <span class="banner-time-wrap-unit">hours</span>
        </div>
        <span class="colon">:</span>
        <div class="banner-time-wrap">
          <span class="banner-time-wrap-number">20</span>
          <span class="banner-time-wrap-unit">minutes</span>
        </div>
        <span class="colon">:</span>
        <div class="banner-time-wrap">
          <span class="banner-time-wrap-number">11</span>
          <span class="banner-time-wrap-unit">second</span>
        </div>
      </div>
      <p class="banner-desc">We will back to something amazing. Getting the latest updates about our games. Please sign up to our newsletter.</p>
      <div class="banner-wrap-input">
        <input placeholder="Enter your email" class="banner-input"/>
      </div>
    </div>
    <div class="header-fairy-wrapper">
      <img src="/img/fairy.png" alt="fairy"/>
    </div>
  </div>
</template>

<style scoped lang="scss">
  .header {
    background-image: url('/img/bg_banner.jpg');
    background-size: cover;
    background-position: center;
    height: 988px;

    &-top {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      padding: 0 58px 94px 80px;
    }

    &-logo {
      padding-top: 20px;
    }

    &-nav {
      display: flex;
      margin-top: 50px ;

      a {
        color: #fff;
        font-size: 14px;
        text-transform: uppercase;
        font-weight: bold;
        margin-left: 84px;
      }

      .lang-select {
        margin-left: 84px;
      }

      &:first-child {
        margin-left: 0;
      }
    }

    &-fairy-wrapper {
      position: absolute;
      left: 0;
      top: 0;
    }
  }

  .banner {
    margin-top: 132px;
    position: relative;
    z-index: 2;

    &-title {
      font-weight: 900;
      font-size: 80px;
      line-height: 120px;
      text-align: center;
      letter-spacing: 0.6px;
      color: #fff;
    }

    &-desc {
      font-size: 18px;
      line-height: 126%;
      text-align: center;
      color: #fff;
      max-width: 560px;
      margin: 0 auto;
    }

    &-wrap-input {
      text-align: center;
      margin-top: 32px;
    }

    &-input {
      width: 560px;
      height: 56px;
      background: #fff;
      border-radius: 8px;
      border: none;
      padding: 18px 14px;
      outline: none;
    }

    &-time {
      width: 756px;
      background-color: #fff;
      margin: 0 auto;
      display: flex;
      padding: 30px 39px;
      box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.25);
      border-radius: 21px;
      justify-content: space-between;
      margin-bottom: 93px;

      &-wrap {
        text-align: center;
        width: 25%;

        &-number {
          font-weight: bold;
          font-size: 60px;
          line-height: 64px;
          text-align: center;
          letter-spacing: 4.8px;
          color: #000;
          display: block;
          text-align: center;
        }

        &-unit {
          font-size: 15.6px;
          line-height: 19px;
          text-align: center;
          letter-spacing: -0.651724px;
          color: #000;
          font-weight: bold;
        }
      }

      .colon {
        font-weight: bold;
        font-size: 60px;
        line-height: 64px;
        text-align: center;
        letter-spacing: 4.8px;
        color: #000;
      }
    }
  }

  @media (max-width: 768px) {
    .header {
      padding: 20px 16px;
      height: 700px;

      &-top {
        flex-direction: row;
        padding: 0;
      }

      &-nav {
          display: none;
      }

      &-fairy-wrapper {
        position: relative;
      }
    }

    .banner {
      margin-top: 44px;

      &-title {
        font-size: 40px;
        line-height: 50px;
        letter-spacing: 0.6px;
        margin-bottom: 38px;
      }

      &-input {
        width: 100%;
      }

      &-time {
        width: 100%;
        padding: 26px 24px;
        margin-bottom: 40px;

        &-wrap {
          &-number {
            font-size: 36px;
            line-height: 45px;
          }

          &-unit {
            font-size: 12px;
            line-height: 15px;
            letter-spacing: -0.651724px;
          }

          &-input {
            margin-top: 16px;
          }
        }

        .colon {
          font-size: 36px;
          line-height: 45px;
        }
      }
    }
  }
</style>

<script>
import { locales, LOCALE_KEY } from "../local_config";

export default {}
</script>
