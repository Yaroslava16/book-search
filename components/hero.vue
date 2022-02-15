<template>
  <section class="hero">
    <h1 class="hero__title">Book search</h1>
    <form class="hero__form">
      <input type="text" placeholder="book title..." />
      <button type="submit"></button>
    </form>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.hero {
  padding: 6vw;
  width: 100%;
  height: 50vh;
  background-image: url(~/assets/hero_BG.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  &__title {
    text-align: center;
    font-size: 4vw;
    font-style: italic;
    font-weight: 700;
    // text-transform: uppercase;
    color: #fff;
  }
  &__form {
    position: relative;
    width: 40vw;
    margin: 0 auto;
    input {
      padding: 1vw;
      width: 100%;
      font-size: 2vw;
      border-radius: 3vw;
      border: 0.3vw solid rgb(255, 208, 0);
      outline: none;
    }
    button {
      position: absolute;
      top: 0;
      right: 0;
      width: 5vw;
      height: 5vw;
      border: 0.3vw solid black;
      background: #ffe066;
      border-radius: 50%;
      cursor: pointer;
      transition: 0.7s;
      &:before {
        content: "🔍";
        font-family: FontAwesome;
        font-size: 16px;
        color: #f9f0da;
      }
      &:hover {
        transform: scale(1.2);
      }
    }
  }
}

.d1 button {
  position: absolute;
  top: 0;
  right: 0px;
  width: 42px;
  height: 42px;
  border: none;
  background: #7ba7ab;
  border-radius: 0 5px 5px 0;
  cursor: pointer;
}
.d1 button:before {
  content: "\f002";
  font-family: FontAwesome;
  font-size: 16px;
  color: #f9f0da;
}
</style>
