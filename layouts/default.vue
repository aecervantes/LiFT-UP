<template>
  <div>
    <header>
      <div class="logo-section">
        <div class="container">
          <div class="row">
            <div class="col">
                <div>
                    <a href="/" class="logo">
                      <img src="LiFT_UP_logo.PNG" alt="LiFT_UP_logo">
                    </a>
                </div>
            </div>
          </div>
        </div>
      </div>

      <site-navigation />
    </header>

    <div class="py-5" id="main">
      <nuxt />
    </div>

    <footer>
      <div class="container-fluid">
        &copy; Aleck Cervantes
      </div>
    </footer>
  </div>
</template>

<script>
import SiteNavigation from "~/components/SiteNavigation";

export default {
  components: {
    SiteNavigation
  }
}
</script>

<style>
  #main{
    font-size:2rem;
  }
</style>