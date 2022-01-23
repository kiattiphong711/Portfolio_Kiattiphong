<template>
  <div class="h-30 w-30 p-4 border-4">
    <p class="text-5xl">Profile</p>
    <br>
        <img
          src="https://media.discordapp.net/attachments/759732616839954442/934732193975136296/193251162_2366947253449198_6339644919942573651_n.png?width=261&height=464"
        />
        <br>
        <span class="block text-4xl">{{ fullName }}</span>
        <span class="block text-4xl">{{ position }}</span>
        <br>
        <span class="block text-3xl font-bold">Education</span>
        <p class="font-bold">Present</p>
        <p>Bangkok University</p>
        <span class="block text-3xl font-bold">Skills</span>
        <ul class="list-inside list-disc">
          <li v-for="skill in skills" :key="skill.id">{{ skill.name }}</li>
        </ul>
        <span class="block text-3xl font-bold">Softwares</span>
        <ul class="list-inside list-disc">
          <li v-for="sw in softwares" :key="sw.id">{{ sw.name }}</li>
        </ul>
        <router-link :to="{ name: 'contact' }">
          <span class="block text-3xl font-bold mb-10 mt-10"
            >Contact me.<img
              class="float-left mr-5"
              src="https://img.icons8.com/ios/50/000000/info--v1.png"
          /></span>
        </router-link>
  </div>
</template>

<script>
import { useRoute } from 'vue-router/dist/vue-router.esm-bundler';

export default {
  data() {
    return {
      fullName: 'Kiattiphong Srangsut',
      position: 'Developer',
      skills: [{ id: 1, name: 'PHP' }],
      softwares: [
        { id: 1, name: 'Adobe Premiere' },
        { id: 2, name: 'Adobe Photoshop' },
        { id: 3, name: 'Adobe After effect' },
      ],
    };
  },
};
</script>
