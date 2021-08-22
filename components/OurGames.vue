<template>
  <section class="our-games">
    <h3 class="our-games-title">Our Games</h3>
    <p class="our-games-desc">As a pioneer of mobile app gamification, we take pride in originality and individuality, providing global players with state-of-the-art games that feature splendid storylines, sensational sound effects and magnificent animation that never cease to impress.</p>
    <ul id="array-rendering" class="our-games-list">
      <li v-for="(item, i) in data" :key="i" :style="{ backgroundImage: `url(${item.bg})` }" class="our-games-list-item">
        <div class="our-games-list-item-wrapper">
          <h5 class="our-games-list-item-title">{{item.tile}}</h5>
          <p class="our-games-list-item-desc">{{item.description}}</p>
        </div>
      </li>
    </ul>
  </section>
</template>

<style scoped lang="scss">
  .our-games {

    padding: 0 60px;
    margin: 100px 0;

    &-title {
      font-size: 60px;
      line-height: 60px;
      font-weight: bold;
      letter-spacing: 3.6px;
      color: #000;
      text-align: center;
      margin-bottom: 25px;
    }

    &-desc {
      font-size: 14px;
      line-height: 20px;
      margin: 0 auto;
      color: #757575;
      max-width: 860px;
      text-align: center;
      margin-bottom: 60px;
    }

    &-list {
      display: flex;
      flex-direction: row;
      flex-wrap: wrap;
      justify-content: center;
      margin: 0 auto;

      &-item {
        max-width: 410px;
        width: 23%;
        height: 560px;
        background-repeat: no-repeat;
        background-position: center;
        display: flex;
        align-items: flex-end;
        margin: 20px;
        padding: 0 32px 40px;
        border-radius: 15px;


        &-title {
          font-weight: bold;
          font-size: 48px;
          line-height: 60px;
          letter-spacing: -1px;
          color: #fff;
          margin-bottom: 15px;
        }

        &-desc {
          font-size: 14px;
          line-height: 20px;
          color: #fff;
        }
      }

      &-item:nth-child(2n) {
        margin-top: 115px;
      }
    }
  }

  @media (max-width: 768px) {
    .our-games {
      padding: 50px 16px 40px;
      margin: 0;

      &-title {
        font-size: 40px;
        line-height: 50px;
        letter-spacing: 0.6px;
      }

      &-desc {
        margin-bottom: 40px;
      }

      &-list {
        justify-content: space-around;

        &-item {
          max-width: 100%;
          width: 164px;
          margin: 0;
          padding: 0 18px 11px 8px;
          height: 268px;

          &-title {
            font-size: 24px;
            line-height: 30px;
          }

          &-decs {
            font-size: 12px;
            line-height: 15px;
            letter-spacing: 0.9px;
          }
        }

        &-item:nth-child(2n) {
        margin-top: 20px;
        }
      }
    }
  }
</style>

<script>
  export default {
  data(){
    return {
      data: [
        {
          tile: 'E-Space',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
          bg: "/img/e_space.jpg"
        },
        {
          tile: 'Kingland',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
          bg: "/img/kingland.jpg"
        },
        {
          tile: 'The Last Game',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
          bg: "/img/lastgame.jpg"
        },
        {
          tile: 'G-Dragon',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
          bg: "img/g_dragon.jpg"
        },
        {
          tile: 'Pirates',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
          bg: "/img/pirates.jpg"
        },
        {
          tile: 'Witch Party',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
          bg: "/img/wicth_party.jpg"
        },
        {
          tile: 'Rocky',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
          bg: "/img/rocky.jpg"
        },
        {
          tile: 'Blue Fire',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
          bg: "/img/blue_fire.jpg"
        },
        {
          tile: 'Magic tree',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
          bg: "/img/magic.jpg"
        },
        {
          tile: 'Aborigines',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
          bg: "/img/aborigines.jpg"
        },
        {
          tile: 'Cinderella',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
          bg: "/img/cinderella.jpg"
        },
        {
          tile: 'Egypt Game',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
          bg: "/img/egyptgame.jpg"
        },
      ]
    }
  }
}
</script>
