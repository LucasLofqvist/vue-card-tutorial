<script setup>
import { ref } from "vue";

const listOfTips = ref([
  {
    adjective: "Lightweight",
    description:
      "I am incredibly small and fast! My core library is only around 30KB, so I won't slow you down.",
  },
  {
    adjective: "Approachable",
    description:
      "Easy to learn and use, even for beginners. I have a gentle learning curve, clear documentation, and a supportive community.",
  },
  {
    adjective: "Versatile",
    description:
      "I can handle everything from simple interactive elements to complex single-page applications. I'm great for small projects and large-scale applications alike.",
  },
]);
</script>

<template>
  <main>
    <section>
      <h2>
        I'm <span class="highlight">{{ listOfTips[0].adjective }}</span>
      </h2>
      <p>
        {{ listOfTips[0].description }}
      </p>
    </section>
    <section>
      <h2>
        I'm <span class="highlight">{{ listOfTips[1].adjective }}</span>
      </h2>
      <p>
        {{ listOfTips[1].description }}
      </p>
    </section>
    <section>
      <h2>
        I'm <span class="highlight">{{ listOfTips[2].adjective }}</span>
      </h2>
      <p>
        {{ listOfTips[2].description }}
      </p>
    </section>
  </main>
</template>

<style scoped>
main {
  margin-top: 15px;
}

section {
  margin-top: 25px;
}

h2 {
  font-size: 1.3rem;
  color: #34495e;
  margin-bottom: 3px;
}

p {
  font-size: 0.9rem;
  color: #555;
}
</style>
