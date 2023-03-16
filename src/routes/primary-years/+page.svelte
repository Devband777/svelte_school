<script>
  import Logo from "$lib/images/Logo.png";
  import Footer from "../../components/footer.svelte";
  import Button from "../../components/button.svelte";
</script>

<svelte:head>
  <title>Primary Years</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>
<div class="primary-years">
  <nav>
    <div class="logo">
      <!-- svelte-ignore a11y-missing-attribute -->
      <img src={Logo} />
    </div>
  </nav>
  <section class="hero">
    <div class="intro-text">
      <h1>
        <span> Primary Years </span> <br />
        <span> Programme</span>
      </h1>
      <p>
        The IB Primary Years Programme (PYP) for children aged 3 – 12 nurtures
        and develops young students as caring, active participants in a lifelong
        journey of learning
      </p>
    </div>
  </section>
  <section class="intro">
    <div class="content">
      <div class="title">Primary Years Programme at Bloomingdale</div>
      <div class="paragraph">
        The IB Primary Years Programme (PYP) for children aged 3 – 12 nurtures
        and develops young students as caring, active participants in a lifelong
        journey of learning.Through its inquiry-led, trans-disciplinary
        framework, the PYP challenges students to think for themselves and take
        responsibility for their learning as they explore local and global
        issues and opportunities in real-life contexts. The PYP Playlist is an
        introduction for parents and teachers who are new to the Primary Years
        Programme. It contains a wide range of e-learning resources to help
        everyone in the learning community develop a deeper understanding of the
        programme, and become more active in supporting student learning. For
        more information: www.ibo.org
      </div>
    </div>
  </section>
  <section class="point">
    <h1 class="title">Learners in the BIS</h1>
    <p class="subtitle">The Primary Years Programme at BIS aims to</p>
  </section>
  
  <Footer />
</div>

<style lang="scss">
  .primary-years {
    nav {
      position: absolute;
      top: 0;
      left: 0;
      z-index: 1;
      margin: 0;
      width: 100%;
      height: 88px;
      display: block;
      flex-direction: row;
      align-items: center;
      padding: 24px 60px;
      gap: 804px;

      .logo {
        width: 206px;
        height: 32px;
        /* Inside auto layout */
        flex: none;
        order: 0;
        flex-grow: 0;
      }
    }
    .hero {
      position: absolute;
      width: 100%;
      height: 800px;
      left: 0px;
      top: 0px;
      background: linear-gradient(
          270deg,
          rgba(0, 0, 0, 0.7) 0%,
          rgba(0, 0, 0, 0) 100%
        ),
        url("../../lib/images/primary-years.png");

      .intro-text {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        padding: 0px;
        gap: 40px;

        position: absolute;
        width: 536px;
        height: 286px;
        left: 80px;
        top: 306px;

        h1 {
          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 56px;
          line-height: 120%;
          /* or 67px */

          color: #ffffff;
        }

        p {
          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 20px;
          line-height: 140%;
          /* or 28px */

          color: #ffffff;
        }
      }
    }
    .intro {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      padding: 128px 60px 208px;
      gap: 10px;

      position: absolute;
      width: 100%;
      height: 672px;
      left: 0px;
      top: 720px;

      background: linear-gradient(
        180deg,
        #fff0d0 0%,
        #effffd 92.44%,
        #caefff 130.5%
      );
      border-radius: 48px 48px 0px 0px;

      .content {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: flex-start;
        padding: 0px;
        gap: 64px;

        .title {
          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 36px;
          line-height: 120%;
          /* or 43px */

          /* Basic & Secondary/Black */

          color: #1e1515;
          width: 403px;
          height: 129px;
          /* Inside auto layout */
          flex: none;
          order: 0;
          flex-grow: 0;
        }

        .paragraph {
          width: 648px;
          height: 336px;
          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 20px;
          line-height: 140%;
          /* or 28px */

          /* Basic & Secondary/Black */

          color: #1e1515;

          opacity: 0.6;
          /* Inside auto layout */

          flex: none;
          order: 1;
          flex-grow: 0;
        }
      }
    }
    .point {
      position: absolute;
      width: 100%;
      height: 1515px;
      left: 0px;
      top: 1312px;

      /* Basic & Secondary/White */

      background: #ffffff;
      border-radius: 48px;

      .title {
        width: 980px;
        height: 67px;

        /* Desktop/H2 Desktop 56 */

        font-family: "Suisse Intl";
        font-style: normal;
        font-weight: 400;
        font-size: 56px;
        line-height: 120%;
        /* or 67px */

        text-align: center;

        /* Basic & Secondary/Black */

        color: #1e1515;

        /* Inside auto layout */

        flex: none;
        order: 0;
        flex-grow: 0;
      }

      .subtitle {
        width: 840px;
        height: 28px;

        /* Desktop/Body Desktop | 20 */

        font-family: "Suisse Intl";
        font-style: normal;
        font-weight: 400;
        font-size: 20px;
        line-height: 140%;
        /* identical to box height, or 28px */

        text-align: center;

        /* Basic & Secondary/Black */

        color: #1e1515;

        opacity: 0.6;

        /* Inside auto layout */

        flex: none;
        order: 1;
        flex-grow: 0;
      }
    }
  }
</style>
