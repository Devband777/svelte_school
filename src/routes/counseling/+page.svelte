<script>
// @ts-nocheck

  import Logo from "$lib/images/Logo.png";
  import VisualImg from "$lib/images/Visual.png";
  import Footer from "../../components/+footer.svelte";
  import Feedback from "../../components/Cards/Feedback.svelte";
  import Collapse from "../../components/+Collapse.svelte";
  import Admission from "../../components/+admission.svelte";
  import Navbar from "../../components/Navbar/+navbar.svelte";
  let collapse_content_1 =
    "<p>Learning as a holistic process, addressing physical, emotional, social and cognitive dimensions</p>" +
    "<p>Building readiness for Primary Years Programme</p>" +
    "<p>Small, learner-centric classes, allowing facilitators to address the specific needs of each child</p>";
</script>

<svelte:head>
  <title>Counseling</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>
<div class="early-years">
  <Navbar/>
  <section class="hero">
    <div class="intro-text">
      <div class="title">Counseling</div>
      <div class="desc">
        Our Career and Guidance Department helps students identify suitable
        career paths, provides exposure to local and global opportunities, and
        guides them in university selection and college applications.
      </div>
    </div>
  </section>
  <section class="intro">
    <div class="content">
      <div class="title">Opportunities for every student</div>
      <div class="paragraph">
        Our Career and Guidance Department helps every student to explore
        possibilities – ones that go in tandem with their respective skills and
        abilities. This not only exposes them to a wide range of opportunities –
        both in India and abroad – but also helps them choose the right
        universities and guides them in the college application filling
        process.  <br /><br />We are regularly in touch with reputed
        universities from India and abroad – in the process, opening up a world
        of opportunities for every student.
      </div>
    </div>
  </section>
  <section class="point">
    <div>
      <div class="title">Key focus of the Career and Guidance Department</div>
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
  <section class="intro2">
    <div class="content">
      <div class="title">Student Support Programme</div>
      <div class="paragraph">
        We have a Student Support Programme which supports the needs of students
        with different learning abilities and needs. A team of specially trained
        educators work with our learners individually and in a group setting,
        enabling as well as equipping them with life skills that are crucial for
        healthy emotional development and growth. There are multiple forums
        where these special educators deliver explicit lessons that teach social
        and emotional skills.<br /><br />At the Bloomingdale International
        School, the emotional well-being of our students is of prime importance.
        Today with the growing challenges, the better we are able to manage our
        emotions, the greater will be our capacity to enjoy life, cope with
        stress, and focus on priorities.<br /><br /> It is for this reason that we
        lay emphasis on developing an emotionally intelligent student.
      </div>
    </div>
  </section>
  <section class="visual">
    <div class="content">
      <div class="left">
        <img src={VisualImg} />
      </div>
      <div class="right">
        <h1>Circle Time</h1>
        <p>
          To help students deal with daily stressors, develop adequate life
          skills and learn effective coping mechanisms, we have Circle Time
          classes for our learners. During this forum, they express their
          thoughts, views and opinions on various topics while also learning how
          to deal with problematic situations positively. The goal at every
          stage is to equip our learners with self-regulatory mechanisms,
          develop a positive self-image, enhance their strengths, and grow into
          well-integrated, resilient individuals. This strengthens their
          emotional health and hones their social skills considerably.
        </p>
      </div>
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
  <Admission top_value="4953px" />
  <Footer top_value="5559px" />
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
        url("../../lib/images/img.png");

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
      top: 3117px;

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
      height: 1116px;
      left: 0px;
      top: 3973px;

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
