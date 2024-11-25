<template>
  <header class="header">
    <img src="@/src/assets/logo.png" alt="logo" />
    <div class="header__wrapper">
      <ul>
        <li>
          <a href="/"><IWhatsapp /> </a>
        </li>
        <li>
          <a href="tel:+7 700 001 18 88"
            ><IPhone /> <span>+7 700 001 18 88</span></a
          >
        </li>
      </ul>
      <ul>
        <li>О проекте</li>
        <li>Локация</li>
        <li>Преимущества</li>
        <li>Почему мы?</li>
        <li>Способы оплаты</li>
        <li>Контакты</li>
      </ul>
    </div>
  </header>
</template>

<script setup>
import IPhone from "../elements/icons/IPhone.vue";
import IWhatsapp from "../elements/icons/IWhatsapp.vue";
</script>

<style lang="scss">
.header {
  display: flex;
  justify-content: space-between;

  img {
    width: 144px;
    height: auto;
  }

  ul {
    &:first-child {
      font-size: 20px;
      letter-spacing: 0.04em;
      display: grid;
      grid-template-columns: repeat(2, max-content);
      grid-gap: 35px;

      a {
        display: flex;
        align-items: center;
      }

      span {
        margin-left: 10px;
      }
    }

    &:last-child {
      margin-top: 16px;
      display: grid;
      grid-template-columns: repeat(6, max-content);
      grid-gap: 50px;
      justify-content: flex-end;
    }
  }

  &__wrapper {
    padding: 25px 0;
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    justify-content: center;
  }
}
</style>
