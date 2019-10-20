<template>
  <div class="container">
    <div>
      <h1 class="title item">What is LiFT UP?</h1>
      <div class="container">
        <h2>Carousel Example</h2>
      </div>

      <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
        <ol class="carousel-indicators">
          <li
            data-target="#carouselExampleIndicators"
            v-for="(slide, index) in slides"
            :data-slide-to="index"
            :class="{'active' : index === 0}"
          ></li>
        </ol>
        <div class="carousel-inner">
          <div
            class="carousel-item"
            v-for="(slide, index) in slides"
            :class="{'active' : index === 0}"
          >
            <div class="slide-image" :style="{'background-image': 'url(' + slide.url + ')'}">
              <img :src="slide.url" :alt="slide.alt" class="sr-only" />
            </div>
          </div>
        </div>
        <a
          class="carousel-control-prev"
          href="#carouselExampleIndicators"
          role="button"
          data-slide="prev"
        >
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="sr-only">Previous</span>
        </a>
        <a
          class="carousel-control-next"
          href="#carouselExampleIndicators"
          role="button"
          data-slide="next"
        >
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="sr-only">Next</span>
        </a>
      </div>
      <p>
        The LiFT UP (Li-Fraumeni TP53 Understanding Penetrance) Study aims to find tools to determine if an individual’s TP53 mutation was acquired or inherited, and to learn more about cancer risk for these individual’s and their family members. Ultimately, this study will increase understanding for how to personalize care for the purposes of early detection and prevention of individuals and their relatives.
        The LiFT UP study specifically aims to:
        <li>Characterize cancer risk for families with Li-Fraumeni syndrome</li>
        <li>Evaluate genetic modifiers of the TP53 gene and their impact on cancer risk</li>
        <li>Determine the frequency of acquired TP53 mutations and its impact on cancer risk and overall healt</li>
      </p>

      <form>
        <button type="submit" formaction="INSERT LINK TO ABOUT TAB">More Info</button>
      </form>

      <form>
        <button type="submit" formaction="INSERT LINK TO REDCAP">Participate</button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      slides: [
        {
          url:
            'https://images.unsplash.com/photo-1534534502714-2828e7c540d0?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2785&q=80',
          alt: 'T-Rex Bones'
        },
        {
          url:
            'https://images.unsplash.com/photo-1532187863486-abf9dbad1b69?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1350&q=80',
          alt: 'Tubes'
        },
        {
          url:
            'https://images.unsplash.com/photo-1481627834876-b7833e8f5570?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1082&q=80',
          alt: 'Library'
        }
      ]
    }
  }
}
</script>

<style>
.carousel-item .slide-image {
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  width: 100%;
  height: 0;
  padding-bottom: 50%;
}
</style>
