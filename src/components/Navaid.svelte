<style>
  .nav-aid,
  .nav-aid > * {
    visibility: hidden;
    opacity: 0;
    display: none;
    transition: all 0.5s ease;
  }

  @media (min-width: 750px) {
    .nav-aid,
    .nav-aid > * {
      visibility: unset;
      opacity: 1;
      display: block;
      z-index: 20;
    }
    .nav-aid {
      position: fixed;
      top: 42%;
      right: 2%;
    }
    .nav-aid > * {
      width: 20px;
      height: 20px;
      border-radius: 100%;
      background: #c7c7c7;
      margin: 8px;
    }

    .aid:hover {
      background: #111010;
      transform: scale(1.2);
      transition: all 0.5s ease; 
      clip-path: polygon(
        50% 0%,
        90% 20%,
        100% 60%,
        75% 100%,
        25% 100%,
        0% 60%,
        10% 20%
      );
    }
  }
</style>

<div class="nav-aid">
  <div class="aid" />
  <div class="aid" />
  <div class="aid" />
  <div class="aid" />
</div>
