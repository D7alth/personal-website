<template>
    <section class="hero">
      <div class="container-hero-content">
        <h1>FullStack Developer</h1>
        <h3 class="signature">Alberth Henrique</h3>
        <div class="container-short-description-text-box">
          <p>Apaixonado por tecnologia desde muito jovem, ao longo dos anos, tenho acumulado experiência em diversos projetos, empresas e desafios. No entanto, minha paixão pela tecnologia nunca diminuiu. Seja atuando em UI/UX, desenvolvimento de Backend, Frontend ou até mesmo em GameDev, cada novo projeto me faz sentir como se fosse a primeira vez.</p>
        </div>  
        <Button link="https://github.com/d7alth" brandingStyle="grow github-branding-button" :icon="['fab', 'github']" text="Ver todos projetos"></Button>
      </div>
        <circular-animated-text>
          <p class="animated-text">Scroll to discover | Scroll to discover |  Scroll to discover |  </p>
        </circular-animated-text>
    </section>
</template>

<style scoped>
.hero{
  background: url("@/assets/images/background-hero.webp") no-repeat center center/cover;
  min-height: 94vh;
  width: 100%;
  align-content: center;
  display: flex;
  justify-content: center;
  flex-direction: column;
  border-radius: 0 0 20px 20px;
}
.container-hero-content{
  max-width: 1100px;
  margin: 4rem auto 0;
}
.container-short-description-text-box
{
  max-width: 630px;
  margin-bottom: 2.4rem;
}
@font-face {
  font-family: 'GalleryModern';
  src: url('@/assets/fonts/GalleryModern.otf') format('opentype');
  font-weight: normal;
  font-style: normal;
}
.signature {
  font-family: var(--font-signature),serif;
  font-size: 4.0rem;
  font-weight: 500;
  text-align: end;
  color: var( --vt-c-red-deep);
  transform: translateY(2rem) rotate(-2deg);
  z-index: 1;
}
h1 {
  font-size: 8rem;
  text-align: center;
  margin-top: 2rem;
  line-height: 0;
}
.animated-text{
  color: var(--vt-c-white);
  font-size: 0.8rem;
  font-weight: bold;
  word-spacing: 0.1rem;
  text-transform: uppercase;
}

.github-branding-button{
  background-color: var(--github-button-color);
  border: none;
  padding: 0.7rem 1.2rem;
  border-radius: 0.2rem;
  font-size: 1.1rem;
  font-family: var(--font-text-simple-1), sans-serif;
  color: var(--vt-c-white);
  font-weight: 600;
  text-transform: capitalize;
  cursor: pointer;
}
</style>
<script setup lang="ts">
import CircularAnimatedText from "@/components/ui/CircularAnimatedText.vue";
import Button from "@/components/ui/Button.vue";
</script>