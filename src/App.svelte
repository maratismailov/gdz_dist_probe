<script>
  import { Route, active } from "tinro";
  import Location from "./components/Location.svelte";
  import Photo from "./components/Photo.svelte";
  import L1 from "./components/L1.svelte";
</script>

<style>

</style>

<main>
  <div class="scrollmenu">
    <a href="/" use:active exact>L_1</a>
    <!-- <a href="/location" use:active exact>Location</a>
    <a href="/photo" use:active exact>Photo</a> -->
  </div>

</main>

<Route path="/photo">
  <Photo />
</Route>
<Route path="/location">
  <Location />
</Route>
<Route path="/">
  <L1 />
</Route>
<!-- <Route path="/currentdustazure">
  <CurrentDustAzure />
</Route>
<Route path="/heatmap">
  <Heatmap />
</Route> -->
