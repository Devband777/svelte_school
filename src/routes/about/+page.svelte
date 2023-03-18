<script>
  // @ts-nocheck

  import Logo from "$lib/images/Logo.png";
  import ChairmanImg from "$lib/images/chairman.png";
  import VisualImg from "$lib/images/middle-visual.png";
  import HistoryImg from "$lib/images/about-histroy.png";

  import Footer from "../../components/+footer.svelte";
  import Feedback from "../../components/Cards/Feedback.svelte";
  import Navbar from "../../components/Navbar/+navbar.svelte";
  let collapse_content_1 =
    "<p>Learning as a holistic process, addressing physical, emotional, social and cognitive dimensions</p>" +
    "<p>Building readiness for Primary Years Programme</p>" +
    "<p>Small, learner-centric classes, allowing facilitators to address the specific needs of each child</p>";
</script>

<svelte:head>
  <title>About</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>
<div class="early-years">
  <Navbar />
  <section class="hero">
    <div class="intro-text">
      <div class="title">Our mission has meaning</div>
      <div class="desc">
        Empower every child's potential through innovative education, fostering
        a diverse and respectful community of learners who promote reflection
        and proactive citizenship.
      </div>
    </div>
  </section>
  <section class="history">
    <div class="content">
      <div class="left">
        <!-- svelte-ignore a11y-missing-attribute -->
        <img src={HistoryImg} />
      </div>
      <div class="right">
        <h1>Our History</h1>
        <p>
          Bloomingdale International School was founded in 2006 as Bloomingdale
          playschool. With the growing need for alternative education practices
          in the city, Bloomingdale then took up the mighty responsibility to
          make children today fall in love with learning and equip them to be
          life-long learners with the foundation of the international curriculum
          and global mindset – thus giving rise to Bloomingdale International
          School in 2016.<br /><br />Bloomingdale is an IB PYP and IB MYP
          Authorized School, which is preferred by the top universities across
          the globe.
        </p>
      </div>
    </div>
  </section>
  <section class="bloomingdable-facts" />
  <section class="visual">
    <div class="content">
      <div class="left">
        <img src={HistoryImg} />
      </div>
      <div class="right">
        <h1>Principal’s message</h1>
        <p>
          Bloomingdale International School was founded in 2006 as Bloomingdale
          playschool. With the growing need for alternative education practices
          in the city, Bloomingdale then took up the mighty responsibility to
          make children today fall in love with learning and equip them to be
          life-long learners
        </p>
      </div>
    </div>
  </section>
  <section class="visual2">
    <div class="content">
      <div class="left">
        <h1 class="title">Chairman's Message</h1>
        <p class="desc">
          It has been an exciting and fulfilling journey to be able to steer the
          quality of life in Vijayawada by educating generations here. It is
          disturbing to know of families parting with their little ones and
          sending them to Boarding Schools to provide International standard
          education.
        </p>

        <p class="footer">
          Viyaya Babu Atluri <br />
          <span>Chairman</span>
        </p>
      </div>
      <div class="right"><img src={ChairmanImg} /></div>
    </div>
  </section>
  <section class="teachers">
    <div class="header">Awesome teachers with great knowleges</div>
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
  <section class="visual3">
    <div class="content">
      <div class="left">
        <img src={VisualImg} />
      </div>
      <div class="right">
        <h1>Principal’s message</h1>
        <p>
          Bloomingdale International School was founded in 2006 as Bloomingdale
          playschool. With the growing need for alternative education practices
          in the city, Bloomingdale then took up the mighty responsibility to
          make children today fall in love with learning and equip them to be
          life-long learners
        </p>
      </div>
    </div>
  </section>
  <Footer top_value="8094px" />
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
        url("../../lib/images/middle-years-hero.png");

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
    .history {
      position: absolute;
      width: 100%;
      height: 936px;
      left: 0px;
      top: 720px;

      /* Brandcolors/Mint */

      background: #efdb34;
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
    .bloomingdable-facts {
      position: absolute;
      width: 100%;
      height: 1654px;
      left: 0px;
      top: 1576px;

      /* Basic & Secondary/Gradient Blue & Orange */

      background: linear-gradient(
        180deg,
        #caefff 0%,
        #effffd 23.3%,
        #fff0d0 82.39%
      );
      border-radius: 48px 48px 0px 0px;
      transform: matrix(-1, 0, 0, 1, 0, 0);
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
    .intro2 {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      box-sizing: border-box;
      padding: 128px 60px;
      gap: 10px;

      position: absolute;
      width: 100%;
      height: 784px;
      left: 0px;
      top: 2413px;

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
      top: 3150px;

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

    .visual2 {
      position: absolute;
      width: 100%;
      height: 936px;
      left: 0px;
      top: 4006px;

      /* Brandcolors/Orange */

      background: #de8a2e;
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
        text-align: left;

        .left {
          display: flex;
          flex-direction: column;
          align-items: flex-start;
          padding: 0px;
          gap: 40px;
          width: 536px;
          height: 471px;
          .title {
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

            color: #fff;
          }
          .desc {
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

            color: #fff;
          }
          .footer {
            font-family: "Suisse Intl";
            font-style: normal;
            font-weight: 500;
            font-size: 32px;
            line-height: 120%;
            /* or 38px */

            text-align: center;

            /* Basic & Secondary/White */

            color: #ffffff;
            span {
              font-family: "Suisse Intl";
              font-style: normal;
              font-weight: 400;
              font-size: 20px;
              line-height: 140%;
              /* identical to box height, or 28px */

              /* Basic & Secondary/White */

              color: #ffffff;
            }
          }
        }
        .right {
          background: url(AAA9793-scaled-1024x532.jpg);
          border-radius: 24px;
          transform: matrix(-1, 0, 0, 1, 0, 0);
        }
      }
    }
    .visual3 {
      position: absolute;
      width: 100%;
      height: 1238px;
      left: 0px;
      top: 7238px;

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
      top: 1228px;

      /* Basic & Secondary/White */

      background: #ffffff;
      border-radius: 48px;

      .title {
        position: absolute;
        top: 128px;
        text-align: center;
        left: 30%;
        right: 30%;
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
      left: 0px;
      top: 5818px;

      height: 1500px;
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

    .teachers {
      position: absolute;
      width: 100%;
      height: 1036px;
      left: 0px;
      top: 4862px;

      background: #ffffff;
      border-radius: 48px;

      box-sizing: border-box;
      padding: 128px 60px;
      .header {
        width: 580px;
        height: 134px;

        /* Desktop/H2 Desktop 56 */

        font-family: "Suisse Intl";
        font-style: normal;
        font-weight: 400;
        font-size: 56px;
        line-height: 120%;
        /* or 67px */

        color: #0f1121;
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

          color: #1e1515;
        }
      }
    }
  }
</style>
