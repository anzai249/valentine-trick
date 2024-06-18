<template>
  <div class="va-container">
    <img src="./assets/ava.png" alt="avatar" class="avatar" />
    <p class="question-text">Will you be my valentine?</p>
    <div class="buttons">
      <vaButton @click="yesClicked" class="yes-button"></vaButton>
      <vaButtonNo
        @click="noClicked"
        @mouseover="noHovered"
        @mouseleave="noLeaved"
        class="no-button"
      ></vaButtonNo>
    </div>
  </div>
</template>

<script>
import vaButton from "./components/va-button.vue";
import vaButtonNo from "./components/va-button-no.vue";
import { gsap } from "gsap";

export default {
  components: {
    vaButton,
    vaButtonNo,
  },
  data() {
    return {
      btnScale: 1,
    };
  },
  mounted() {},
  methods: {
    noClicked() {
      this.btnScale = this.btnScale + 0.5;
      gsap.to(".yes-button", {
        duration: 1,
        scale: this.btnScale,
        ease: "power3",
      });
    },
    noHovered() {
      window.addEventListener("mousemove", this.mouseListener);
    },
    noLeaved() {
      window.removeEventListener("mousemove", this.mouseListener);
    },
    mouseListener(e) {
      gsap.set(".no-button", { xPercent: -50, yPercent: -100 });
      let xTo = gsap.quickTo(".no-button", "x", {
          duration: 0.8,
          ease: "power3",
        }),
        yTo = gsap.quickTo(".no-button", "y", {
          duration: 0.8,
          ease: "power3",
        });
      let windowWidth = window.innerWidth;
      let windowHeight = window.innerHeight;
      xTo(e.clientX - windowWidth / 2);
      yTo(e.clientY - windowHeight / 2);
    },
    yesClicked() {
      alert("I love you!");
    },
  },
};
</script>

<style scoped>
.va-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 10px;
}
.avatar {
  width: 500px;
  margin: 0 auto;
  display: block;
}

.buttons {
  display: flex;
  justify-content: center;
  gap: 20px;
}

.question-text {
  font-size: 1.5em;
  color: white;
  text-align: center;
}
</style>
