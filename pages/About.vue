<template>
  <h1>This is about page</h1>
</template>
<script>
export default {
  heade() {
    return {
      title: "About Page",
      meta:[
        {
            hid:'Description',
            name:'description',
            content:'This is about page',
        }
      ]
    };
  },
};
</script>