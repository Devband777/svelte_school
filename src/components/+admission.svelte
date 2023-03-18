<script>
  import ArrowDown from "$lib/images/arrow-down.png";
  import Arrow from "$lib/images/arrow.png";

  
  export let top_value = "4335px";
</script>

<section class="admission" style="--top_value: {top_value}">
  <div class="title">
    <h1 class="main-title">Admission to Bloomingdale School</h1>
    <p class="sub-title">
      Enter your child’s of birth to discover the key steps and relecant
      information about how to join us
    </p>
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
</section>

<style lang="scss">
  .admission {
    position: absolute;
    width: 100%;
    height: 988px;
    left: 0px;
    top: var(--top_value);

    /* Brandcolors/Orange */
    background: #de8a2e;
    border-radius: 48px;
    box-sizing: border-box;
    padding: 128px 200px;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 80px;

    .title {
      text-align: center;
      width: 600px;
      height: 230px;
      .main-title {
        /* Desktop/H2 Desktop 56 */

        font-family: "Suisse Intl";
        font-style: normal;
        font-weight: 400;
        font-size: 56px;
        line-height: 120%;
        /* or 67px */

        text-align: center;

        /* Basic & Secondary/White */

        color: #ffffff;
      }
      .sub-title {
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
</style>
