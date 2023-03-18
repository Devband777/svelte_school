<script>
  import Logo from "$lib/images/Logo.png";
  import VisualImg from "$lib/images/middle-visual.png";
  import Footer from "../../components/+footer.svelte";
  import Button from "../../components/+button.svelte";
  import Feedback from "../../components/Cards/Feedback.svelte";
  import Collapse from "../../components/+Collapse.svelte";
  import ArrowDown from "$lib/images/arrow-down.png";
  import Arrow from "$lib/images/arrow.png";
  import Admission from "../../components/+admission.svelte";
  import Navbar from "../../components/Navbar/+navbar.svelte";
  
  let collapse_content_1 =
    "<p>Learning as a holistic process, addressing physical, emotional, social and cognitive dimensions</p>" +
    "<p>Building readiness for Primary Years Programme</p>" +
    "<p>Small, learner-centric classes, allowing facilitators to address the specific needs of each child</p>";
</script>

<svelte:head>
  <title>Early Years</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>
<div class="early-years">
  <Navbar/>
  <section class="hero">
    <div class="intro-text">
      <div class="title">Early Years</div>
      <div class="desc">
        At Bloomingdale International School, every detail is designed to ensure
        each child is happy, involved and learning
      </div>
    </div>

    <div class="hero-button">
      <Button
        bk_color="#fff"
        text_color="#1E1515"
        caption="Early Years showreel"
      />
    </div>
  </section>
  <section class="intro">
    <div class="content">
      <div class="title">About Early Years at Bloomingdale</div>
      <div class="paragraph">
        At Bloomingdale International School, every detail is designed to ensure
        each child is happy, involved and learning. Our Early Learning Village
        [Village Campus], located in the heart of Benz Circle, Amaravthi, only 9
        km from BIS Galileo Campus, is built on the simple truth: the
        environment nurtures the child. From AY 2022, our Early Learning Centre
        at the BIS Galileo Campus will also be operational. Our Early Year’
        programme is for the Playgroup only. Primary Years Programme is followed
        from Nursery upwards.<br /><br /> Our Early Years’ architectural experts
        have created exceptional spaces for sensorial learning at every turn on both
        the campuses. Families enjoy the warmth of natural wood timbers and bright
        airy open spaces, to provide endless opportunities to learn, connect and
        belong.
      </div>
    </div>
  </section>
  <section class="visual">
    <div class="content">
      <div class="left">
        <img src={VisualImg} />
      </div>
      <div class="right">
        <h1>Early Years</h1>
        <p>
          Our Early Years Programme creates a unique and engaging learning
          environment. It employs the best of international pedagogies and is
          based on five areas of learning which converge towards our Mind Body
          Soul programme as illustrated here
        </p>
      </div>
    </div>
  </section>
  <section class="point">
    <div>
      <div class="title">
        «Education is not preparation for life, it is Life itself»
      </div>
      <div class="subtitle">
        Our Early Years Programme creates a unique and engaging learning
        environment. It employs the best of international pedagogies and is
        based on five areas of learning which converge towards our Mind Body
        Soul programme as illustrated here. Our areas of emphasis are:
      </div>
    </div>
    <div class="content">
      <div class="left">
        <Collapse caption="Areas of emphasis #1" content={collapse_content_1} />
        <Collapse caption="Areas of emphasis #2" content={collapse_content_1} />
        <Collapse caption="Areas of emphasis #3" content={collapse_content_1} />
      </div>
      <div class="right" />
    </div>
  </section>
  <section class="facts">
    <div class="title">
      <h1 class="main-title">Some facts about Early Years program</h1>
    </div>
  </section>
  <section class="feedback">
    <div class="content">
      <div class="left">
        <div class="title">
          Parents' feedback about our school. We provide an environment where we
          teach students how to think rather than what to think.
        </div>
      </div>
      <div class="right">
        <div class="feedback-cards">
          <Feedback
            content="At Bloomingdale, Performing Arts, Sports and well-being and Life skills are taught too, which are essential for cognitive development and overall growth of the children."
            name1="Mike Kaszuk"
            name2="Parent of Manvitha"
          />
          <Feedback
            content="At Bloomingdale, Performing Arts, Sports and well-being and Life skills are taught too, which are essential for cognitive development and overall growth of the children."
            name1="Mike Kaszuk"
            name2="Parent of Manvitha"
          />
        </div>
      </div>
    </div>
  </section>
  <Admission top_value="5292px" />
  
  <Footer top_value="5898px" />
</div>

<style lang="scss">
  .early-years {
    
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
        url("../../lib/images/early-years-hero.png");

      .hero-button {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        position: absolute;
        width: 536px;
        height: 286px;
        left: -80px;
        top: 480px;
      }
      .intro-text {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        padding: 0px;

        position: absolute;
        width: 536px;
        height: 286px;
        left: 80px;
        top: 313px;

        .title {
          width: 536px;
          height: 134px;

          /* Desktop/H2 Desktop 56 */

          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 56px;
          line-height: 120%;
          /* or 67px */

          color: #ffffff;

          /* Inside auto layout */

          flex: none;
          order: 0;
          flex-grow: 0;
        }

        .desc {
          width: 450px;
          height: 112px;

          /* Desktop/Body Desktop | 20 */

          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 20px;
          line-height: 140%;
          /* or 28px */

          color: #ffffff;

          /* Inside auto layout */

          flex: none;
          order: 1;
          flex-grow: 0;
        }
      }
    }

    .intro {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      box-sizing: border-box;
      padding: 128px 60px;
      gap: 10px;

      position: absolute;
      width: 100%;
      height: 1092px;
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

        left: 4.67%;
        right: 4.67%;
        height: 756px;

        /* Inside auto layout */

        flex: none;
        order: 0;
        flex-grow: 0;

        .title {
          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 36px;
          line-height: 120%;
          /* or 43px */

          /* Basic & Secondary/Black */

          color: #1e1515;
          width: 50%;
          height: 129px;
          /* Inside auto layout */
          flex: none;
          order: 0;
          flex-grow: 0;
        }

        .paragraph {
          width: 50%;
          height: 336px;

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

          /* Inside auto layout */

          flex: none;
          order: 1;
          flex-grow: 0;
        }
      }
    }
    .visual {
      position: absolute;
      width: 100%;
      height: 936px;
      left: 0px;
      top: 2630px;

      /* Brandcolors/Mint */

      background: #a6d6c9;
      border-radius: 48px;
      .content {
        position: absolute;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: flex-start;
        padding: 0px;
        gap: 64px;

        left: 4.67%;
        right: 4.67%;
        height: 336px;
        top: 128px;

        .left {
          background: url(AAA9793-scaled-1024x532.jpg);
          border-radius: 24px;
          transform: matrix(-1, 0, 0, 1, 0, 0);
        }
        .right {
          display: flex;
          flex-direction: column;
          align-items: flex-start;
          padding: 0px;
          gap: 40px;
          width: 536px;
          height: 471px;
          h1 {
            width: 332px;
            height: 67px;

            /* Desktop/H2 Desktop 56 */

            font-family: "Suisse Intl";
            font-style: normal;
            font-weight: 400;
            font-size: 56px;
            line-height: 120%;
            /* or 67px */

            /* Basic & Secondary/Dark Blue */

            color: #254b6a;

            /* Inside auto layout */

            flex: none;
            order: 0;
            flex-grow: 0;
          }
          p {
            width: 536px;
            height: 364px;

            /* Desktop/Body Desktop | 20 */

            font-family: "Suisse Intl";
            font-style: normal;
            font-weight: 400;
            font-size: 20px;
            line-height: 140%;
            /* or 28px */

            /* Basic & Secondary/Dark Blue */

            color: #254b6a;

            /* Inside auto layout */

            flex: none;
            order: 1;
            flex-grow: 0;
          }
        }
      }
    }
    .point {
      position: absolute;
      width: 100%;
      height: 1314px;
      left: 0px;
      top: 1340px;

      /* Basic & Secondary/White */

      background: #ffffff;
      border-radius: 48px;

      .title {
        position: absolute;
        top: 128px;
        text-align: center;
        left: 10%;
        right: 10%;
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
        position: absolute;
        top: 302px;
        left: 30%;
        right: 30%;
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

      .content {
        position: absolute;
        top: 446px;
        left: 4.67%;
        right: 4.67%;
        .left {
          box-sizing: border-box;

          /* Auto layout */

          display: flex;
          flex-direction: column;
          align-items: flex-start;

          width: 50%;
          padding-right: 136px;

          /* Inside auto layout */

          flex: none;
          order: 0;
          align-self: stretch;
          flex-grow: 0;
          float: left;
        }
        .right {
          width: 50%;
          height: 660px;
          top: 0px;
          float: left;
          background-image: url("$lib/images/img_primary_point.png");

          background-repeat: no-repeat;

          border-radius: 24px;

          flex: none;
          order: 1;
          flex-grow: 0;
        }
      }
    }
    .feedback {
      position: absolute;
      width: 100%;
      height: 1116px;
      left: 0px;
      top: 4312px;

      background: linear-gradient(
        360deg,
        #caefff -33.82%,
        #effffd 1.46%,
        #fff0d0 90.94%
      );
      border-radius: 48px;

      .content {
        display: flex;
        align-items: flex-start;
        padding: 0px;
        gap: 162px;

        box-sizing: border-box;

        position: absolute;
        height: 724px;
        left: 4.67%;
        right: 4.67%;
        top: 128px;
        .left {
          width: 50%;
          .title {
            width: 510px;
            height: 215px;

            /* Desktop/H3 Desktop | 36 */

            font-family: "Suisse Intl";
            font-style: normal;
            font-weight: 400;
            font-size: 36px;
            line-height: 120%;
            /* or 43px */

            /* Basic & Secondary/Black */

            color: #1e1515;

            /* Inside auto layout */

            flex: none;
            order: 0;
            flex-grow: 0;
          }
        }

        .right {
          width: 50%;
          .feedback-cards {
            /* Feedback cards */

            /* Auto layout */

            display: flex;
            flex-direction: column;
            align-items: flex-start;
            padding: 0px;
            gap: 48px;

            width: 648px;
            height: 724px;

            /* Inside auto layout */

            flex: none;
            order: 1;
            flex-grow: 0;
            float: right;
          }
        }
      }
    }
    .admission {
      position: absolute;
      width: 100%;
      height: 988px;
      left: 0px;
      top: 5292px;

      /* Brandcolors/Orange */
      background: #de8a2e;
      border-radius: 48px;
      box-sizing: border-box;
      padding: 128px 200px;
      display: flex;
      justify-content: center;
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
    .facts {
      position: absolute;
      width: 100%;
      height: 906px;
      left: 0px;
      top: 3486px;

      /* Basic & Secondary/White */

      background: #ffffff;
      border-radius: 48px;
      box-sizing: border-box;
      padding: 128px 200px;
      display: flex;
      justify-content: center;
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

          color: #1E1515;
        }
      }
    }
  }
</style>
