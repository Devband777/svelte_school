<script>
  import Button from "./button.svelte";
</script>

<section class="footer">
  <section class="footer">
    <div class="navigation">
        <div class="email-input">
            <h1>Keep Learning</h1>
            <p>Subscribe to Bloomingdale updates</p>
            <input type="text" placeholder="Enter youe email here*" />
        </div>
        <div class="menu">

        </div>
    </div>
  </section>
  <section class="cta">
    <p>Unlock your child's potential — apply to join today!</p>
    <Button bk_color="#fff" text_color="#64A8DF" caption="Enquiry" />
  </section>
</section>

<style lang="scss">
  .footer {
    position: absolute;
    width: 100%;
    height: 1080px;
    left: 0px;
    top: 4335px;

    .cta {
      position: absolute;
      left: 4.17%;
      right: 4.17%;
      top: 0%;
      bottom: 64.63%;

      /* Brandcolors/Blue */

      background: #64a8df;
      border-radius: 48px;

      p {
        position: absolute;
        width: 1013px;
        height: 134px;
        left: 153px;
        top: 72px;

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

      Button {
        margin-left: 592px;
        margin-top: 254px;
        
      }
    }

    .footer {
      position: absolute;
      left: 0%;
      right: 0%;
      top: 17.69%;
      bottom: 0%;

      /* Basic & Secondary/Black */

      background: #1e1515;
      border-radius: 48px 48px 0px 0px;
    }
  }
</style>
