<script>
  import BackgroundImg from "$lib/images/img.png";
  import Logo from "$lib/images/Logo.png";
  import Burger from "$lib/images/Burger.png";
  // import Input from "../../components/Input.svelte"
  import ArrowDown from "$lib/images/arrow-down.png";
  import Arrow from "$lib/images/arrow.png";
  import Footer from "../../components/+footer.svelte";
  import Navbar from "../../components/Navbar/+navbar.svelte";
</script>

<svelte:head>
  <title>Transport</title>
  <meta name="description" content="School Life/Transport" />
</svelte:head>

<div class="transport">
  <Navbar />
  <div class="hero">
    <img src={BackgroundImg} class="img" />
    <span class="title-subtitle">
      <span class="title"> Transport </span>
      <span class="subtitle">
        All our busses are equipped with AC, built-in GPS and safety equipment.
        We hire an experienced team to ensure students safety
      </span>
    </span>
  </div>
  <div class="intro-list">
    <div class="content">
      <span class="intro-title"> Transport </span>
      <span class="intro-content">
        Starting for the academic year 2021-22 Parents will be able to get alert
        as the bus is about to reach the designated stop. Parents will also be
        able to track child's location through a mobile App
      </span>
    </div>
  </div>
  <div class="admission">
    <div class="content">
      <div class="title-subtitle">
        <span class="title"> Admission to Bloomingdale School </span>
        <span class="subtitle">
          Enter your child’s of birth to discover the key steps and relecant
          information about how to join us
        </span>
      </div>
      <div class="tabs-button">
        <button class="dropdown-button">
          Day
          <img src={ArrowDown} class="arrow-down" />
        </button>
        <button class="dropdown-button">
          Month
          <img src={ArrowDown} class="arrow-down" />
        </button>
        <button class="dropdown-button">
          Year
          <img src={ArrowDown} class="arrow-down" />
        </button>
        <button class="btn">
          Calculate
          <img src={Arrow} class="arrow" />
        </button>
      </div>
    </div>
  </div>
  <Footer />
</div>

<style lang="scss">
  .transport {
    .hero {
      .img {
        position: absolute;
        width: 100%;
        left: 0px;
        top: 0px;
        background: linear-gradient(
          90deg,
          rgba(0, 0, 0, 0.7) -0.45%,
          rgba(0, 0, 0, 0.28) 100%
        );
      }

      .button {
        box-sizing: border-box;
      }

      .title-subtitle {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: flex-start;
        padding: 0px;
        gap: 40px;

        position: absolute;
        width: calc(100% * 470 / 1440);
        height: calc(100% * 191 / 800);
        left: calc(4%);
        top: calc(50%);

        .title {
          width: 245px;
          height: 67px;
          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 56px;
          line-height: 120%;
          color: #ffffff;
        }

        .subtitle {
          width: 470px;
          height: 84px;
          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 20px;
          line-height: 140%;
          color: #ffffff;
        }
      }
    }

    .intro-list {
      position: absolute;
      width: 100%;
      height: calc(100% / 800 * 1164);
      left: 0px;
      top: calc(100% / 800 * 720);
      background: linear-gradient(
        180deg,
        #caefff -24.83%,
        #effffd 7.42%,
        #fff0d0 89.22%
      );
      border-radius: 48px 48px 0px 0px;

      .content {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: flex-start;
        padding: 0px;
        gap: calc(100% / 1440 * 64);

        position: absolute;
        width: calc(100% / 1440 * 1320);
        height: calc(100% / 800 * 84);
        left: calc(100% / 1440 * 60);
        top: calc(100% / 800 * 128);

        .intro-title {
          width: 312px;
          height: 43px;

          /* Desktop/H3 Desktop | 36 */

          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 36px;
          line-height: 120%;
          /* or 43px */

          /* Basic & Secondary/Black */

          color: #1e1515;
        }

        .intro-content {
          width: 648px;
          height: 84px;

          /* Desktop/Body Desktop | 20 */

          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 20px;
          line-height: 140%;
          /* or 28px */

          /* Basic & Secondary/Black */

          color: #1e1515;

          opacity: 0.6;
        }
      }
    }

    .admission {
      /* Section | Admission */
      position: absolute;
      width: 100%;
      height: calc(100% / 800 * 988);
      left: 0px;
      top: calc(100% / 800 * 1804);

      /* Brandcolors/Orange */
      background: #de8a2e;
      border-radius: 48px;

      .content {
        /* Auto layout */
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 0px;
        gap: 64px;

        position: absolute;
        width: calc(100% / 1440 * 645);
        height: calc(100% / 800 * 350);
        left: calc(100% / 1440 * 398);
        top: calc(100% / 800 * 128);

        .title-subtitle {
          /* Auto layout */
          display: flex;
          flex-direction: column;
          align-items: center;
          padding: 0px;
          gap: 40px;
          width: 600px;
          height: 230px;

          /* Inside auto layout */
          flex: none;
          order: 0;
          flex-grow: 0;

          .title {
            width: 600px;
            height: 134px;

            /* Desktop/H2 Desktop 56 */
            font-family: "Suisse Intl";
            font-style: normal;
            font-weight: 400;
            font-size: 56px;
            line-height: 120%;
            /* or 67px */
            text-align: center;
            color: #fff;
          }

          .subtitle {
            width: 460px;
            height: 56px;

            /* Desktop/Body Desktop | 20 */
            font-family: "Suisse Intl";
            font-style: normal;
            font-weight: 400;
            font-size: 20px;
            line-height: 140%;
            /* or 28px */
            text-align: center;

            /* Basic & Secondary/White */
            color: #ffffff;
          }
        }

        .tabs-button {
          /* Auto layout */
          display: flex;
          flex-direction: row;
          align-items: flex-start;
          padding: 0px;
          gap: 8px;
          width: 645px;
          height: 56px;

          .dropdown-button {
            box-sizing: border-box;

            /* Auto layout */
            display: flex;
            flex-direction: row;
            justify-content: center;
            align-items: center;
            padding: 16px 48px;
            gap: 10px;
            background: transparent;

            width: 148px;
            height: 56px;

            border: 2px solid rgba(255, 255, 255, 0.6);
            border-radius: 100px;
            color: #ffffff;

            .arrow-down {
              /* arrow-down */
              width: 15px;
              height: 15px;
            }
          }

          .btn {
            /* Auto layout */
            display: flex;
            flex-direction: row;
            align-items: center;
            padding: 12px 12px 12px 24px;
            gap: 12px;

            width: 152px;
            height: 56px;

            /* Basic & Secondary/White */
            background: #ffffff;
            border-radius: 100px;
            border: none;

            /* Desktop/btn1 Desktop | 16 */
            font-family: "Suisse Intl";
            font-style: normal;
            font-weight: 500;
            font-size: 16px;
            line-height: 100%;
            /* identical to box height, or 16px */

            /* Brandcolors/Orange */
            color: #de8a2e;

            .arrow {
              width: 32px;
              height: 32px;
            }
          }
        }
      }
    }
  }
</style>
