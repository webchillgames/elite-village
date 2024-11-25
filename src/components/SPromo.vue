<script setup>
import EButton from "../elements/EButton.vue";
import CHeader from "./CHeader.vue";
</script>

<template>
  <section id="promo" class="promo">
    <div class="promo__wrapper wrapper">
      <CHeader />

      <div class="promo__content">
        <div>
          <h2>Элитный коттеджный городок в г. Нур-Султан</h2>
          <EButton>Скачать презентацию</EButton>

          <div class="promo__houses-info">
            <p>36 коттеджей</p>
            <ul>
              <li>
                <p>3</p>
                <p>
                  коттеджа <br />
                  368 м<sup>2</sup> <br />
                  на 10 сотках
                </p>
              </li>
              <li>
                <p>33</p>
                <p>
                  коттеджа <br />
                  179 м<sup>2</sup> <br />на 5 сотках
                </p>
              </li>
            </ul>
          </div>
        </div>

        <ul class="promo__deadlines">
          <li>
            <span>Строительные работы </span>начались в сентября 2021 года.
          </li>
          <li><span>Срок сдачи</span> коттеджей - I квартал 2022 года</li>
          <li>
            <span>Срок сдачи</span> всего коттеджного городка - II квартал 2022
            года
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<style lang="scss">
.promo {
  background-image: url("@/src/assets/promo-bg.jpg");
  background-color: $accent;
  background-size: cover;
  background-repeat: no-repeat;
  color: $text;
  height: 736px;

  a {
    color: inherit;
  }

  h2 {
    font-weight: 700;
    font-size: 38px;
    line-height: 140%;
    margin-bottom: 20px;
  }

  button {
    padding: 20px 30px;
    background-color: $accent-light;
    color: $text-dark;
    font-weight: 700;
    margin-bottom: 40px;
  }

  &__wrapper {
    display: grid;
    grid-template-rows: max-content 1fr;
  }

  &__content {
    padding-top: 115px;
    display: grid;
    grid-template-columns: 1fr max-content;
    grid-gap: 42px;
  }

  &__deadlines {
    display: grid;
    grid-template-rows: repeat(3, max-content);
    grid-gap: 30px;
    max-width: 300px;

    span {
      font-weight: 700;
    }
  }

  &__houses-info {
    p {
      font-weight: 700;
      font-size: 32px;
      line-height: 140%;
    }

    ul {
      margin-top: 20px;
    }

    ul,
    li {
      display: grid;
      grid-template-columns: repeat(2, max-content);
      align-items: flex-start;
    }

    ul {
      grid-gap: 26px;
    }

    li {
      grid-gap: 20px;
      p:first-child {
        font-weight: 400;
        font-size: 128px;
        line-height: 84%;
      }

      p:last-child {
        font-weight: 400;
        font-size: 20px;
        line-height: 140%;
      }
    }
  }
}
</style>
