<script>
  import { mode } from "../util/store";
  import { onMount } from "svelte";
</script>

<style>
  .content {
    flex-flow: column nowrap;
  }

  .myself {
    border-radius: 100%;
  }

  .description {
    font-size: 24px;
    text-align: center;
  }

  .info {
    font-size: 14px;
    padding: 8px;
  }

  .dark {
    filter: grayscale(1);
  }

  @media (min-width: 750px) {
    .content {
      flex-flow: row nowrap;
    }

    .description {
      font-size: 34px;
      padding: 0px 10px;
      font-family: "Fira Code", monospace;
    }

    .info {
      font-size: 18px;
    }
  }
</style>

<section 
  class="swiper-slide flex-center content"
  data-hash="javascript">
  <div class="description">
    <p>
      Full Stack Developer
      <img src="/assets/img/verify.svg" alt="verified" />
    </p>
    <p class="info">
      I design and develop
      <span class="keyword">wonderful∞</span>
      apps
    </p>
  </div>
  <div>
    <picture>
      <source
        srcset="/assets/img/bruno_edoh_large.png"
        media="(min-width: 750px)" />
      <img
        class={`myself ${$mode}`}
        src="/assets/img/bruno_edoh_small.png"
        alt="bruno edoh" />
    </picture>
  </div>
</section>
