<template>
  <section class="about-us">
    <div class="about-us-content sub-container">
      <div class="about-us-content-left">
        <h3 class="about-us-title">About Us</h3>
        <p class="about-us-desc">Browse our selection of free online games and have a great time without leaving the site! Our Kids Games option also includes game reviews, extensive game cheats and walkthroughs, and much more. We have exclusive free downloads, videos, and articles as well. Etech reviews the most popular kids games from all the most popular video gaming platforms, so you don’t need to search around for fun anywhere else on the Internet. Explore a whole new world of gaming on Etech.</p>
        <div class="about-us-info">
          <p class="about-us-item"><span>600M+</span> Users</p>
          <p class="about-us-item"><span>135+</span> Games</p>
        </div>
      </div>
      <div class="about-us-content-right">
        <div class="wrapper">
          <div class="img">
            <img src="/img/calendar-tick.png" alt="">
          </div>
          <div class="wrapper-content">
            <h4 class="wrapper-title">24 - Hour</h4>
            <p class="wrapper-desc">24/7 access ensures operators' businesses runs smoothly all year long.</p>
          </div>
        </div>
        <div class="wrapper">
          <div class="img">
            <img src="/img/pen-tool-2.png" alt="">
          </div>
          <div class="wrapper-content">
            <h4 class="wrapper-title">Design</h4>
            <p class="wrapper-desc">Combining imaginative universes, play dynamics, and unprecedented gameplay, our games transcend the boundaries of the virtual world by weaving innovative gameplay.</p>
          </div>
        </div>
        <div class="wrapper">
          <div class="img">
            <img src="/img/people.png" alt="">
          </div>
          <div class="wrapper-content">
            <h4 class="wrapper-title">Team</h4>
            <p class="wrapper-desc">Etech is an award-winning, international studio of designers, artists, animators and producers that create content for the biggest names in film and video games. </p>
          </div>
        </div>
      </div>
    </div>
    <div class="sub-container about-us-bg">
        <img src="/img/Illustrator.png" alt="" class="about-us-bg-first-img"/>
        <img src="/img/bg_map.jpg" alt="" class="about-us-bg-second-img"/>
      </div>
  </section>
</template>

<style scoped lang="scss">
  .about-us {
    padding-top: 128px;
    position: relative;

    &-content {
      display: flex;
      flex-direction: row;
      justify-content: space-between;

      &-left {
        width: 560px;
      }

      &-right {
        width: 560px;
        background-color: #eee;
        padding-top: 113px;
        padding-left: 74px;
      }
    }

    &-title {
      font-size: 60px;
      line-height: 60px;
      font-weight: bold;
      letter-spacing: 3.6px;
      color: #000;
      margin-bottom: 40px;
    }

    &-desc {
      font-size: 14px;
      line-height: 20px;
      color: #757575;
      margin-bottom: 80px;
    }

    &-item {
      font-weight: bold;
      font-size: 24px;
      line-height: 30px;
      color: #000;
      margin-bottom: 39px;

      span {
        font-size: 80px;
        line-height: 98px;
        letter-spacing: -1px;
        color: #079BEE;
        display: block;
      }
    }

    &-bg {
      margin-top: 398px;

      &-first-img {
        position: absolute;
        bottom: 327px;
        margin-left: auto;
        margin-right: auto;
        left: 0;
        right: 0;
        text-align: center;
      }
    }
  }

  .wrapper {
    display: flex;
    flex-direction: row;
    margin-bottom: 40px;

    .img {
      width: 50px;
      height: 50px;
      border-radius: 25px;
      background-color: #e3fcff;
      display: flex;
      justify-content: center;
      align-items: center;
      margin-right: 24px;

      img {
        width: 24px;
        height: auto;
      }
    }

    &-content {
      max-width: 336px;
    }

    &-title {
      font-size: 24px;
      line-height: 30px;
      font-weight: bold;
      color: #000;
      margin-bottom: 9px;
    }

    &-desc {
      font-size: 14px;
      line-height: 20px;
      color: #757575;
    }
  }

  .wrapper:last-child {
    margin-bottom: 0;
  }

  @media (max-width: 768px) {
    .about-us {
      margin-top: 340px;
      padding: 0 16px;

      &-title {
        margin-bottom: 16px;
      }

      &-desc {
        margin-bottom: 30px;
      }

      &-info {
        display: flex;
      }

      &-item {
        font-size: 24px;
        line-height: 30px;

        span {
          font-size: 44px;
          line-height: 54px;
          letter-spacing: -1px;
        }
      }

      &-item:first-child {
        margin-right: 55px;
      }

      &-content {
        flex-direction: column;

        &-left {
          width: 100%;
        }

        &-right {
          width: 100%;
          padding: 40px 20px;
        }
      }

      &-bg {
        margin-top: 260px;
        position: relative;

        &-first-img {
          width: 300px;
          bottom: 0;
          top: -200px;
        }
      }
    }

    .wrapper {
      .img {
        min-width: 50px;
      }
    }
  }
</style>

<script>
export default {}
</script>
