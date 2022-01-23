<template>
  <div class="h-30 w-30 p-4 border-4">
    <p class="text-5xl mb-10">Contact</p>
    <ul>
      <li>
        <span class="block text-3xl mb-10">0969746954
        <img
            class="float-left mr-5"
            src="https://img.icons8.com/external-sbts2018-blue-sbts2018/50/000000/external-contact-social-media-basic-1-sbts2018-blue-sbts2018.png"
        /></span>
      </li>
      <li>
        <span class="block text-3xl mb-10">
          Kiattiphong Srangsut<img
            class="float-left mr-5"
            src="https://img.icons8.com/color/48/000000/facebook-new.png"
          />
        </span>
      </li>
      <li>
        <span class="block text-3xl mb-10">kiattiphong.sran@bumail.net
        <img
          class="float-left mr-5"
          src="https://img.icons8.com/color/50/000000/gmail-new.png"
        />
            </span>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import { useRoute } from 'vue-router/dist/vue-router.esm-bundler';
export default {
  name: 'Contact',
  setup() {
    const route = useRoute();
  },
};
</script>

