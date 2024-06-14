<template>
  <div>
    <section id="projects" class="py-12 md:py-24">
      <div class="max-w-5xl mx-auto px-4 lg:px-10">
        <div class="lg:py-3">
          <LineItem title="Our Projects" />
        </div>
        <div class="lg:pl-3 flex flex-col lg:flex-row lg:items-end">
          <h1
            class="flex lg:w-[50%] shrink-0 flex-col md:flex-row capitalize lg:flex-col text-4xl font-bold tracking-tightest leading-none"
          >
            <span class="text-black">Here is What we </span>
            <span class="text-[#0071BC] md:pl-1.5 lg:pl-0">have worked on</span>
          </h1>
        </div>

        <div class="py-5 lg:py-10">
          <div
            class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-5 lg:px-4"
          >
            <ProjectItem
              title="Solar energy"
              body="Solar water pumping project carried out at Rhino camp in Arua District."
              url="images/solar.webp"
            />

            <ProjectItem
              title="Boreholes and clean water"
              body="Project Beneficiaries accessing clean water at Bidibidi Refuge Settlement camp - Yumbe District."
              url="images/project-2.jpg"
            />

            <ProjectItem
              title="Building and infrastructure"
              body="Construction of VIP Latrines."
              url="images/project-3.jpg"
            />
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import ProjectItem from "./Projects/ProjectItem.vue";
export default {
  components: {
    ProjectItem,
  },
};
</script>
