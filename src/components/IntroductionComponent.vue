<template>
  <div>
    <div class="media">
      <div class="media__image animate-wiggle">
        <img class="introduction-image" src="../assets/svg/The-big-idea.webp" alt="" />
        <img class="arrow" src="../assets/svg/arrow.svg" alt="" />
      </div>

      <div class="media__body" data-aos="fade-right" data-aos-duration="900">
        <h2 class="media__header">
          Introduction to getlinked <span class="color-purple">tech Hackathon 1.0</span>
        </h2>
        <p class="media__text">
          Our tech hackathon is a melting pot of visionaries, and its purpose is as clear as day: to
          shape the future. Whether you're a coding genius, a design maverick, or a concept wizard,
          you'll have the chance to transform your ideas into reality. Solving real-world problems,
          pushing the boundaries of technology, and creating solutions that can change the world,
          that's what we're all about!
        </p>
      </div>

      <img src="../assets/svg/Purple-Lens-Flare.svg" alt="" class="blur-three" />

      <!--  -->

      <img class="absolute__items-1" src="../assets/icons/star.svg" alt="" />
      <img class="absolute__items-2" src="../assets/icons/star1.svg" alt="" />
      <img class="absolute__items-3" src="../assets/icons/star2.svg" alt="" />
      <img class="absolute__items-4" src="../assets/icons/satagra.svg" alt="" />
    </div>
  </div>
</template>

<script></script>

<style lang="scss" scoped>
.media {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 109px;
  border: 1px solid rgba(255, 255, 255, 0.18);
  border-top: none;
  border-left: 0;
  border-right: 0;
  height: auto;
  padding-top: 62px;
  padding-bottom: 78px;

  @media screen and (max-width: 992px) {
    flex-direction: column;
    height: auto;
    text-align: center;
    gap: 58px;
    padding-left: 48px;
    padding-right: 48px;
    padding-top: 29px;
    padding-bottom: 40px;
  }

  .media__image {
    position: relative;
    animation-iteration-count: infinite;
    animation-name: wiggle;
    animation-duration: 2s;
    animation-timing-function: ease-in-out;
    .introduction-image {
      max-width: 490px;

      @media screen and (max-width: 768px) {
        width: 264px;
      }
    }

    .arrow {
      position: absolute;
      right: 0;
      animation-iteration-count: infinite;
      animation-name: wiggle;
      animation-duration: 1s;
      // animation-timing-function: ease-in-out;
      @media screen and (max-width: 768px) {
        width: 29.456px;
      }
    }

    @keyframes wiggle {
      0%,
      100% {
        transform: rotate(-5deg);
      }
      50% {
        transform: rotate(5deg);
      }
    }
  }

  .media__body {
    @media screen and (max-width: 768px) {
      text-align: center;
    }
    .media__header {
      font-family: Clash Display;
      font-size: 32px;
      font-weight: 700;
      max-width: 398px;
      line-height: 42.56px;
      margin-bottom: 16px;

      @media screen and (max-width: 992px) {
        text-align: center;
        font-size: 20px;
        width: 249px;
        margin: auto;
        margin-bottom: 9px;
        line-height: 133%;
      }

      .color-purple {
        color: #d434fe;
      }
    }
    .media__text {
      font-size: 14px;
      font-weight: 400;
      line-height: 27.5px;
      max-width: 535px;

      @media screen and (max-width: 768px) {
        font-size: 12px;
      }

      .color-pink {
        color: #ff26b9;
        font-weight: 700;
      }

      .text__bold {
        font-weight: 700;
      }
    }
    .margin-bottom {
      margin-bottom: 22px;
    }
  }
}
</style>
