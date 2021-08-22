<template>
   <div>
      <h1>{{ msg }}</h1>
      <n-space horizontal>
         <n-button>Default</n-button>
         <n-button type="primary">Primary</n-button>
         <n-button type="info">Info</n-button>
         <n-button type="success">Success</n-button>
         <n-button type="warning">Warning</n-button>
         <n-button type="error">Error</n-button>
      </n-space>
   </div>
</template>

<script lang="ts">
import { ref, defineComponent } from "vue";

export default defineComponent({
   name: "HelloWorld",
   props: {
      msg: {
         type: String,
         required: true,
      },
   },
   setup: () => {
      const count = ref(0);
      return { count };
   },
});
</script>

<style scoped>
a {
   color: #42b983;
}

label {
   margin: 0 0.5em;
   font-weight: bold;
}

code {
   background-color: #eee;
   padding: 2px 4px;
   border-radius: 4px;
   color: #304455;
}
</style>
