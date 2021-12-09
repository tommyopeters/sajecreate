<template>
  <main class="projects">
    <h1>Hi, I'm Richard Oseghale</h1>
    <p class="description">
      A Skilled and creative graphic designer with a keen eye for aesthetics.
      Acquired industry competency in architecture, concept development, product
      design and illustration, website user interface design and project
      management.
    </p>

    <div class="richard-banner"></div>

    <div class="expertise">
      <span>Program Expertise</span>
      <ul class="expertise-list">
        <li
          class="expertise-list-item"
          v-for="program in programs"
          :key="program.index"
        >
          <div class="image-control">
            <img :src="program.icon" alt="" />
          </div>
          <div class="name">{{ program.name }}</div>
        </li>
      </ul>
    </div>
  </main>
</template>

<script>
export default {
  data() {
    return {
      programs: [
        {
          index: 1,
          icon: "~/assets/images/programs/Photoshop.png",
          name: "Photoshop",
        },
        {
          index: 2,
          icon: "~/assets/images/programs/Illustrator.png",
          name: "Illustrator",
        },
        {
          index: 3,
          icon: "~/assets/images/programs/InDesign.png",
          name: "InDesign",
        },
        {
          index: 4,
          icon: "~/assets/images/programs/XD.png",
          name: "Adobe XD",
        },
        {
          index: 5,
          icon: "~/assets/images/programs/PremierePro.png",
          name: "Premiere Pro",
        },
        {
          index: 6,
          icon: "~/assets/images/programs/AfterEffects.png",
          name: "After Effects",
        },
        {
          index: 7,
          icon: "~/assets/images/programs/Affinity.png",
          name: "Affinity Designer",
        },
        {
          index: 8,
          icon: "~/assets/images/programs/Autocad.png",
          name: "Autocad",
        },
        {
          index: 9,
          icon: "~/assets/images/programs/Revit.png",
          name: "Revit",
        },
        {
          index: 10,
          icon: "~/assets/images/programs/Sketchup.png",
          name: "Sketchup",
        },
      ],
    };
  },
};
</script>
