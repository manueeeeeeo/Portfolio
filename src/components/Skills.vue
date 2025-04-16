<template>
  <section id="skills" class="my-12 animate-fade-in">
    <h2 class="text-3xl font-semibold mb-6">Habilidades</h2>

    <!-- Lenguajes -->
    <h3 class="text-xl font-semibold mb-2">Lenguajes</h3>
    <div class="space-y-4 mb-6">
      <SkillBar name="Java" level="90" />
      <SkillBar name="SQL" level="80" />
      <SkillBar name="Python" level="76" />
      <SkillBar name="C#" level="50" />
      <SkillBar name="JavaScript" level="50" />
    </div>

    <!-- Herramientas -->
    <h3 class="text-xl font-semibold mb-2">Herramientas</h3>
    <div class="space-y-4">
      <SkillBar name="Android Studio" level="100" />
      <SkillBar name="Visual Studio" level="92" />
      <SkillBar name="Firebase" level="86" />
      <SkillBar name="MongoDB" level="65" />
    </div>
  </section>
</template>

<script setup>
const skills = [
  { name: 'Java', level: 90 },
  { name: 'SQL', level: 80 },
  { name: 'Python', level: 76 },
  { name: 'C#', level: 50 },
  { name: 'JavaScript', level: 50 },
  { name: 'Android Studio', level: 100 },
  { name: 'Visual Studio', level: 92 },
  { name: 'Firebase', level: 86 },
  { name: 'MongoDB', level: 65 },
]
</script>

<!-- Componente SkillBar -->
<script>
export default {
  components: {
    SkillBar: {
      props: ['name', 'level'],
      template: `
        <div>
          <div class="flex justify-between text-sm mb-1">
            <span>{{ name }}</span>
            <span>{{ level }}%</span>
          </div>
          <div class="w-full bg-gray-200 rounded-full h-3">
            <div
              class="bg-blue-500 h-3 rounded-full transition-all duration-500"
              :style="{ width: level + '%' }"
            ></div>
          </div>
        </div>
      `,
    },
  },
}
</script>