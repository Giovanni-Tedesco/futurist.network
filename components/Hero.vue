<template>
  <div class="g-landing">
    <div
      class="f-hero d-flex align-content-center justify-content-center flex-column"
    >
      <p class="f-hero-tag">Propose, Fund, & Work.</p>
      <h1 class="f-hero-heading">
        Crowdsourcing
        <br />the
        <span class="text-rainbow">Future.</span>
      </h1>

      <Btn class="mt-5" name="Join Now" />

      <!-- MORE INDICATOR -->
      <div class="more-indicator animation-more mt">
        <fa-icon :icon="['fas', 'angle-double-down']"></fa-icon>
      </div>
    </div>
  </div>
</template>

<style>
.g-landing {
  margin: 0 120px;
}

.text-rainbow {
  color: red;
  background-image: -webkit-linear-gradient(92deg, red, yellow);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  -webkit-animation: hue 10s infinite linear;
}

@-webkit-keyframes hue {
  from {
    -webkit-filter: hue-rotate(0deg);
  }

  to {
    -webkit-filter: hue-rotate(-360deg);
  }
}

.hero-tag {
  font-size: 18px;
  font-weight: 600;
  color: #7c7c7c;
  letter-spacing: 0;
  line-height: 1.5;
  text-align: center;
  font-family: 'Montserrat', sans-serif;
}

.btn {
  z-index: 1;
  padding: 8px 50px;
  border-radius: 30px;
  cursor: pointer;
  font-size: 1em;
  letter-spacing: 2px;
  transition: 0.3s ease;
  font-weight: bold;
  border: none;
  color: white;
}

.btn :hover {
  text-decoration: none;
}

/* ----------- MORE INDICATOR ------------ */
.more-indicator {
  text-align: center;
  font-size: 14px;
  padding: 40px 40px;
  opacity: 0;
  color: white;
  font-weight: bold;
}

.mt {
  margin-top: 20px;
}

/* ANIMATE */
.animation-more {
  animation-name: drive;
  animation-duration: 3s;
  animation-fill-mode: forwards;
  animation-delay: 0.5s;
  animation-iteration-count: infinite;
}

/* KEYFRAMES */
@keyframes drive {
  from {
    transform: translateY(0);
    opacity: 0;
  }

  to {
    transform: translateY(15px);
    opacity: 1;
  }
}
</style>
