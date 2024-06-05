<script setup lang="ts">

import Card from "@/components/ui/Card.vue";
</script>

<template>
  <section class="services">
    <h2 class="services-headline">Especialidades</h2>
    <div class="container services-cards-box">
      <Card title="UI/UX">
        <p>
         Um dos meus pontos fortes e o UI/UX design, 
         tendo trabalhado em dezenas de projetos freelancers, 
         criando interfaces intuitivas e atraentes.
        </p>
      </Card>
      <Card title="Front-End">
        <p>
          Ainda que não considere o front-end a minha especialidade, 
          a maior parte da minha experiencia como progrmador foi com 
          front-end, tendo trabalhado principalemnte com Vue.js e Angular
        </p>
      </Card>
      <Card title="Back-End">
        <p>
          Essa sem duvidas e a area a qual eu me destaco, tendo trabalhado com diversas
          tecnologias e linguagens, como C#, PHP e Node.js. Criei, mantive, otimizei e contribui
          para dezenas de sistemas e APIs, tanto como freelancer quanto apenas por diversão.
        </p>
      </Card>
      <Card title="E mais">
        <p>
          Seja como <b>GameDev</b>, <b>DevOps</b>, <b>Wordpress</b>, <b>Mobile</b> ou <b>devops</b>
          meu objetivo e sempre ir mais longe e me desafiar, seja em projetos pessoais ou profissionais,
          e pretendo ir muito mais longe.
        </p>
      </Card>
    </div>
  </section>
</template>

<style scoped>
.services
{
  max-width: 1100px;
  margin: 8rem auto 4rem;
  padding: 0 1.2rem;
}
.services-cards-box
{
  display: flex;
  flex-wrap: nowrap;
}
.services-headline
{
  font-size: 3rem;
  text-align: left;
  margin-bottom: 1rem;
  font-weight: 500;
  text-transform: capitalize;
  letter-spacing: 0.1rem;

}
</style>