<script>
  import Button from "../components/+button.svelte";
  import Logo from "$lib/images/Logo.png";
  import IBSchoolImg from "$lib/images/img _ IB school.png";
  import IBContinuumImg from "$lib/images/img _ IB Continuum.png";
  import Student1 from "$lib/images/student1.png";
  import Student2 from "$lib/images/student2.png";
   

  export let top_value = "4335px";
</script>

<section class="footer" style="--top_value: {top_value}">
  <section class="footer">
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
    <div class="divider" />
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
  </section>
  <section class="cta">
    <div class="desc">Unlock your child's <span class="students">
        <!-- svelte-ignore a11y-missing-attribute -->
        <img class="stu1" src={Student1}>
        <!-- svelte-ignore a11y-missing-attribute -->
        <img class="stu2" src={Student2}>
      </span> potential — apply to join today!
      
    </div>
    <div><Button bk_color="#fff" text_color="#64A8DF" caption="Enquiry" /></div>
      
  </section>
</section>

<style lang="scss">
  .footer {
    position: absolute;
    width: 100%;
    height: 1080px;
    left: 0px;
    top: var(--top_value);

    .cta {
      position: absolute;
      left: 4.17%;
      right: 4.17%;
      top: 0%;
      bottom: 64.63%;

      box-sizing: border-box;
      padding: 72px 154px;

      /* Brandcolors/Blue */

      background: #64a8df;
      border-radius: 48px;

      text-align: center;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      .desc {
        /* Desktop/H2 Desktop 56 */

        font-family: "Suisse Intl";
        font-style: normal;
        font-weight: 400;
        font-size: 56px;
        line-height: 120%;
        margin-bottom: 20px;
        widows: 1013px;
        /* or 67px */
        /* Basic & Secondary/White */

        color: #ffffff;
      }
    }

    .footer {
      position: absolute;
      left: 0%;
      right: 0%;
      top: 17.69%;
      bottom: 0%;
      width: 100%;
      height: 889px;

      /* Basic & Secondary/Black */

      background: #1e1515;
      border-radius: 48px 48px 0px 0px;

      .navigation {
        position: absolute;
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -ms-flex-wrap: wrap;
        flex-wrap: wrap;
        height: 228px;
        top: 263px;

        left: 4.17%;
        right: 4.17%;

        .email-input {
          -webkit-box-flex: 0;
          -ms-flex: 0 0 50%;
          flex: 0 0 50%;
          width: 50%;

          display: -webkit-box;
          display: -ms-flexbox;
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
          display: -webkit-box;
          display: -ms-flexbox;
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
        position: absolute;
        width: 100%;
        height: 0px;
        left: 0px;
        top: 555px;

        border: 1px solid rgba(255, 255, 255, 0.2);
      }
      .campus-info {
        position: absolute;
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -ms-flex-wrap: wrap;
        flex-wrap: wrap;
        top: 619px;
        height: 206px;

        left: 4.17%;
        right: 4.17%;

        .left {
          width: 50%;
          .logo {
            position: absolute;
            width: 206px;
            height: 32px;
            left: 60px;
            top: 0;
          }
          div {
            position: absolute;
            width: 350px;
            height: 44px;
            left: 60px;
            top: 55px;

            /* Desktop/Body 2 Desktop | 16 */

            font-family: "Suisse Intl";
            font-style: normal;
            font-weight: 400;
            font-size: 16px;
            line-height: 140%;
            /* or 22px */

            color: rgba(255, 255, 255, 0.5);
          }
          .ib {
            .school {
              position: absolute;
              width: 56px;
              height: 56px;
              left: 0px;
              top: 120px;
            }
            .continuum {
              position: absolute;
              width: 72px;
              height: 56px;
              left: 68px;
              top: 120px;
            }
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

            position: absolute;
            width: 434px;
            height: 118px;
            left: 50%;
            top: 0;

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
