<script lang="ts">
  import { Router, Route } from "svelte-navigator"
  import Articles from "src/pages/Articles.svelte"
  import InvestingAdvice from "./pages/InvestingAdvice.svelte"
  import MyFavoriteFrontendFramework from "./pages/MyFavoriteFrontendFramework.svelte"
  import VuevsAngular from "./pages/VuevsAngular.svelte"
  import ReactvsSvelte from "./pages/ReactvsSvelte.svelte"
  import Home from "./pages/Home.svelte"
  import Navbar from "./components/Navbar.svelte"
  import Pokemon from "./pages/Pokemon.svelte"
  import SinglePokemon from "./pages/SinglePokemon.svelte"
</script>

<Router>
  <Navbar />
  <Route path="/">
    <Home />
  </Route>
  <Route path="/pokemon">
    <Pokemon />
  </Route>
  <Route path="/pokemon/:id">
    <SinglePokemon />
  </Route>
  <Route path="/articles">
    <Articles />
  </Route>
  <Route path="/investing-advice">
    <InvestingAdvice />
  </Route>
  <Route path="/my-favorite-frontend-framework">
    <MyFavoriteFrontendFramework />
  </Route>
  <Route path="/vue-vs-angular">
    <VuevsAngular />
  </Route>
  <Route path="/react-vs-svelte">
    <ReactvsSvelte />
  </Route>
</Router>

<style global lang="postcss">
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
</style>
