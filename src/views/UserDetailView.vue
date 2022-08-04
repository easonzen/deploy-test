<template>
  <div class="user-detail">
    <h1>user id: {{ id }}</h1>
  </div>
</template>

<script>
import { defineComponent } from "vue";
import { useRoute } from "vue-router";

export default defineComponent({
  setup() {
    const route = useRoute();

    console.log(route.params.id);

    return {
      id: route.params.id,
    };
  },
});
</script>
