<script>
  import { Link, Router, Route } from 'yrv';
</script>

<div class="font-inter flex flex-grow h-screen justify-center items-center">
  <p>
    <Router>
      <Route exact>Hello World</Route>
      <Route fallback>Not found</Route>
      <Route exact path="/:name" let:router>Hey {router.params.name}!</Route>
    </Router>
  </p>
</div>
