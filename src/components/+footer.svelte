<script>
  import Button from "../components/+button.svelte";
  import Logo from "$lib/images/Logo.png";
  import IBSchoolImg from "$lib/images/img _ IB school.png";
  import IBContinuumImg from "$lib/images/img _ IB Continuum.png";
  import Student1 from "$lib/images/student1.png";
  import Student2 from "$lib/images/student2.png";
</script>

<section class="footer-cta">
  <div class="cta">
    <div class="desc">
      Unlock your child's <span class="students">
        <!-- svelte-ignore a11y-missing-attribute -->
        <img class="stu1" src={Student1} />
        <!-- svelte-ignore a11y-missing-attribute -->
        <img class="stu2" src={Student2} />
      </span> potential — apply to join today!
    </div>
    <div><Button bk_color="#fff" text_color="#64A8DF" caption="Enquiry" /></div>
  </div>
  <div class="footer">
    <div class="navigation">
      <div class="email-input">
        <div class="title">Keep Learning</div>
        <div class="input-group">
          <!-- svelte-ignore a11y-label-has-associated-control -->
          <label>Subscribe to Bloomingdale updates</label>
          <input type="text" placeholder="Enter youe email here*" />
        </div>
      </div>
      <div class="menu">
        <div class="main-menu">
          <ul>
            <li>Home</li>
            <li>About Us</li>
            <li>Academics</li>
            <li>School Lofe</li>
            <li>Careers</li>
            <li>Contact Us</li>
          </ul>
        </div>
        <div class="sub-menu">
          <ul>
            <li>After School</li>
            <li>After School</li>
            <li>After School</li>
          </ul>
        </div>
      </div>
    </div>
    <div class="divider"></div>
    <div class="campus-info">
      <div class="left">
        <div class="logo">
          <!-- svelte-ignore a11y-missing-attribute -->
          <img src={Logo} />
        </div>
        <div>
          Bloomingdale International School is a candidate school* for the
          Diploma Programme.
        </div>
        <div class="ib">
          <!-- svelte-ignore a11y-missing-attribute -->
          <img class="school" src={IBSchoolImg} />
          <!-- svelte-ignore a11y-missing-attribute -->
          <img class="continuum" src={IBContinuumImg} />
        </div>
      </div>
      <div class="right">
        <div class="campus">
          <div class="campus-1">
            <h1>Campus 1</h1>
            <p class="des">Fishponds Road Penamaluru</p>
            <p class="phone">T. +91 7569303221</p>
          </div>
          <div class="campus-2">
            <h1>Campus 2</h1>
            <p class="des">Fishponds Road Penamaluru</p>
            <p class="phone">T. +91 7569303221</p>
          </div>
        </div>
        <div class="social-media" />
      </div>
    </div>
  </div>
</section>

<style lang="scss">
  .footer-cta {
    flex-direction: column;
    height: auto;
    overflow: hidden;
    .cta {
      position: relative;
      top: 181px;
      z-index: 2;
      box-sizing: border-box;
      padding: 72px 154px;

      background: #64a8df;
      border-radius: 48px;

      text-align: center;

      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      margin: 0 auto;

      width: 80%;
      height: 382px;

      .desc {
        font-family: "Suisse Intl";
        font-style: normal;
        font-weight: 400;
        font-size: 56px;
        line-height: 120%;
        margin-bottom: 48px;
        width: 1013px;
        color: #ffffff;
      }
    }

    .footer {
      position: relative;
      z-index: 1;
      width: 100%;
      height: 889px;

      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;

      box-sizing: border-box;
      padding: 60px;

      background: #1e1515;
      border-radius: 48px 48px 0px 0px;

      .navigation {
        margin-top: 170px;
        display: flex;
        -ms-flex-wrap: wrap;
        flex-wrap: wrap;
        height: 228px;
        width: 100%;

        .email-input {
          -webkit-box-flex: 0;
          -ms-flex: 0 0 50%;
          flex: 0 0 50%;
          width: 50%;

          display: flex;
          -ms-flex-wrap: wrap;
          flex-wrap: wrap;

          .title {
            font-family: "Suisse Intl";
            font-style: normal;
            font-weight: 400;
            font-size: 36px;
            line-height: 120%;
            color: #fafafa;

            /* Inside auto layout */

            flex: none;
            order: 0;
            flex-grow: 0;

            width: 100%;
          }

          .input-group {
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            padding: 0px;
            gap: 12px;

            width: 100%;
            height: 85px;

            /* Inside auto layout */

            flex: none;
            order: 1;
            flex-grow: 0;

            label {
              font-family: "Suisse Intl";
              font-style: normal;
              font-weight: 400;
              font-size: 14px;
              line-height: 120%;
              /* identical to box height, or 17px */

              color: rgba(255, 255, 255, 0.8);

              /* Inside auto layout */

              flex: none;
              order: 0;
              flex-grow: 0;
            }
            input {
              display: flex;
              flex-direction: row;
              align-items: center;
              padding: 14px 32px;
              gap: 12px;

              width: 400px;
              height: 56px;

              background: rgba(255, 255, 255, 0.1);
              border-radius: 100px;
              border: none;

              color: #fff;

              /* Inside auto layout */

              flex: none;
              order: 1;
              flex-grow: 0;
            }
          }
        }

        .menu {
          display: flex;
          -ms-flex-wrap: wrap;
          flex-wrap: wrap;
          -ms-flex: 0 0 50%;
          flex: 0 0 50%;
          width: 50%;
          .main-menu {
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            padding: 0px;
            gap: 12px;
            isolation: isolate;
            gap: 20px;

            color: #fafafa;
            -webkit-box-flex: 0;
            -ms-flex: 0 0 66.666667%;
            flex: 0 0 66.666667%;
            width: 66.666667%;

            display: -webkit-box;
            display: -ms-flexbox;
            display: flex;
            -ms-flex-wrap: wrap;
            flex-wrap: wrap;

            font-family: "Suisse Intl";
            font-style: normal;
            font-weight: 500;
            font-size: 20px;
            line-height: 140%;
            ul {
              list-style: none;
              width: 106px;
              height: 228px;
            }
          }
          .sub-menu {
            -webkit-box-flex: 0;
            -ms-flex: 0 0 33.333333%;
            flex: 0 0 33.333333%;
            width: 33.333333%;

            color: rgba(255, 255, 255, 0.8);

            font-family: "Suisse Intl";
            font-style: normal;
            font-weight: 400;
            font-size: 14px;
            line-height: 120%;
            ul {
              list-style: none;
            }
          }
        }
      }
      .divider {
        border: 1px solid rgba(255, 255, 255, 0.2);
        width: 200%;
        margin: 65px -60px;
      }
      .campus-info {
        display: flex;
        -ms-flex-wrap: wrap;
        flex-wrap: wrap;
        width: 100%;
        .left {
          width: 50%;
          div {
            font-family: "Suisse Intl";
            font-style: normal;
            font-weight: 400;
            font-size: 16px;
            line-height: 140%;
            color: rgba(255, 255, 255, 0.5);
            margin-bottom: 30px;
          }
        }
        .right {
          width: 50%;

          .campus {
            display: flex;
            flex-direction: row;
            align-items: flex-start;
            padding: 0px;
            gap: 48px;

            .campus-1 {
              h1 {
                font-family: "Suisse Intl";
                font-style: normal;
                font-weight: 500;
                font-size: 20px;
                line-height: 140%;
                /* identical to box height, or 28px */

                color: #ffffff;
              }

              .des {
                font-family: "Suisse Intl";
                font-style: normal;
                font-weight: 400;
                font-size: 16px;
                line-height: 140%;
                /* or 22px */

                color: rgba(255, 255, 255, 0.8);
              }

              .phone {
                font-family: "Suisse Intl";
                font-style: normal;
                font-weight: 400;
                font-size: 16px;
                line-height: 140%;
                /* or 22px */

                color: rgba(255, 255, 255, 0.8);
              }
            }
            .campus-2 {
              h1 {
                font-family: "Suisse Intl";
                font-style: normal;
                font-weight: 500;
                font-size: 20px;
                line-height: 140%;
                /* identical to box height, or 28px */

                color: #ffffff;
              }

              .des {
                font-family: "Suisse Intl";
                font-style: normal;
                font-weight: 400;
                font-size: 16px;
                line-height: 140%;
                /* or 22px */

                color: rgba(255, 255, 255, 0.8);
              }

              .phone {
                font-family: "Suisse Intl";
                font-style: normal;
                font-weight: 400;
                font-size: 16px;
                line-height: 140%;
                /* or 22px */

                color: rgba(255, 255, 255, 0.8);
              }
            }
          }
        }
      }
    }
  }
</style>
