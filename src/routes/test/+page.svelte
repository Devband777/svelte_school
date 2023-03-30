<script>
  import gsap from "gsap";
  import ScrollTrigger from "gsap/ScrollTrigger";

  import { onMount } from "svelte";


  // image import
  onMount(() => {
    gsap.registerPlugin(ScrollTrigger);

    const timeline = gsap.timeline({
      scrollTrigger: {
        trigger: ".section-2",
        start: "top top",
        end: "+=200%",
        scrub: true,
        pin: true,
        anticipatePin: 1,
        markers: true,
      },
    });
    timeline.to(".section-2 h1", { duration: 1, rotate: 360 });
  });
</script>

<svelte:head>

</svelte:head>

<style lang="scss">
  :global(body) {
    margin: 0;
  }

  section {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
  }

  .section-2 {
    // display: flex;
    // align-items: center;
    // justify-content: center;
    // min-height: 100vh;
    background: lightgrey;
  }

  .section-2 h1 {
    color: teal;
  }
  .section-3 {
    // display: flex;
    // align-items: center;
    // justify-content: center;
    // min-height: 100vh;
    background: papayawhip;
  }

  .section-3 h1 {
    color: salmon;
  }
</style>
