<template>
  <section class="our-partners">
    <h3 class="our-partners-title">Our Partners</h3>
    <ul class="our-partners-list container">
      <li class="our-partners-list-item">
        <img src="/img/ea_game.png" alt="" />
      </li>
      <li class="our-partners-list-item">
        <img src="/img/game.png" alt="" />
      </li>
      <li class="our-partners-list-item">
        <img src="/img/power.png" alt="" />
      </li>
      <li class="our-partners-list-item">
        <img src="/img/disney.png" alt="" />
      </li>
      <li class="our-partners-list-item">
        <img src="/img/bookpro.png" alt="" />
      </li>
    </ul>
  </section>
</template>

<style scoped lang="scss">
  .our-partners {
    background-color: #f6f6f6;
    padding: 120px 0;

    &-title {
      font-weight: bold;
      font-size: 60px;
      line-height: 80px;
      text-align: center;
      letter-spacing: 3.6px;
      color: #000;
      margin-bottom: 80px;
    }

    &-list{
      display: flex;
      flex-direction: row;
    }
  }

  @media (max-width: 768px) {
    .our-partners {
      padding: 40px 16px;

      &-title {
        font-size: 40px;
        line-height: 50px;
        letter-spacing: 0.6px;
        margin-bottom: 40px;
      }
    }
  }
</style>

<script>
export default {}
</script>
