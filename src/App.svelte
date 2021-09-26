<script lang="ts">
  import { Router, Route } from "svelte-routing";
  import "carbon-components-svelte/css/g90.css";
  import { Home, Lesson } from "./pages";
</script>

<Router>
  <main>
    <Route path="" component={Home} />
    <Route path="lesson" component={Lesson} />
  </main>
</Router>

<style>
  main {
    max-width: 1280px;
    width: 90vw;
    margin: 3rem auto;
  }
</style>
