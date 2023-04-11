<template>
  <div>
    <Grid
      h="200px"
      w="200px"
      templateRows="repeat(3, 1fr)"
      templateColumns="repeat(3, 1fr)"
    >
      <GridItem v-for="(item, index) in board" :key="index">{{
        item
      }}</GridItem>
    </Grid>
  </div>
</template>

<script>
import { Grid, GridItem } from "@chakra-ui/vue";
export default {
  name: "CheckBoard",
  components: { Grid, GridItem },
  data() {
    return {
      board: [0, 0, 0, 0, 0, 0, 0, 0, 0],
    };
  },
};
</script>

<style lang="scss"></style>
