<script>
  // @ts-nocheck
  import Herobg from "$lib/images/layer1_back.png";
  import Videobg from "$lib/images/video.png";
  import School from "$lib/images/school.png";
  import Student1 from "$lib/images/student1.png";
  import Student2 from "$lib/images/student2.png";
  import Book from "$lib/images/book1.png";
  import Fomular from "$lib/images/Fomular.png";
  import Paper from "$lib/images/Paper.png";
  import ReasonImg1 from "$lib/images/img1.png";
  import Stroke2Img from "$lib/images/img5.png";
  import Rectangle1 from "$lib/images/rec1.png";
  import Rectangle2 from "$lib/images/rec2.png";
  import Rectangle3 from "$lib/images/rec3.png";
  import Rectangle4 from "$lib/images/rec4.png";
  import Rectangle5 from "$lib/images/rec5.png";
  import Rectangle6 from "$lib/images/rec6.png";
  import Frame from "$lib/images/frame.png";
  import Buttonimg from "$lib/images/Button.png";
  import Card from "../components/Cards/Card.svelte";
  import Card1 from "../components/Cards/Card1.svelte";
  import Button from "../components/+button.svelte";
  import Feedback from "../components/Cards/Feedback.svelte";
  import Navbar from "../components/Navbar/+navbar.svelte";
  import Footer from "../components/+footer.svelte";

  import CompanyLogo1 from "$lib/images/Microsoft-Showcase-School 1.png";
  import CompanyLogo2 from "$lib/images/nba-seeklogo.com 1.png";
  import CompanyLogo3 from "$lib/images/Frame 1000004283.png";
  import CompanyLogo4 from "$lib/images/la-liga-seeklogo.com 1.png";
  import CompanyLogo5 from "$lib/images/image 1554.png";

  import { fade } from "svelte/transition";
  import { gsap } from "gsap";

  import { onMount } from "svelte";

  let ready = false;
  onMount(() => {
    gsap.fromTo(
      ".title",
      {
        opacity: 0,
        y: "50%",
      },
      {
        duration: 0.8,
        opacity: 1,
        y: 0,
        delay: 0.2,
        ease: "Bounce.inOut",
        stagger: 0.1,
      }
    );
  });
</script>

<svelte:head>
  <title>Homepage</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>

<section class="home">
  <Navbar />
  <section class="hero">
    <div class="title-img">
      <span class="title"> The <span style="color: #DE8A2E;">#1</span></span>
      <span class="title">
        <!-- svelte-ignore a11y-missing-attribute -->
        <img src={Student1} class="img1" />
        <!-- svelte-ignore a11y-missing-attribute -->
        <img src={Student2} class="img2" />
        <span class="txt">&nbsp;School for</span>
      </span>
      <span class="title">performers</span>
    </div>
  </section>
  <section class="stroke-video">
    <div class="video">
      <!-- svelte-ignore a11y-missing-attribute -->
      <img src={Videobg} class="img" />
    </div>
    <div class="stroke">
      <!-- svelte-ignore a11y-missing-attribute -->
      <img src={Stroke2Img} class="img1" />
      <span class="text">School for creators</span>
      <span class="text" style="left: -5%;">School for creators</span>
    </div>
  </section>
  <section class="edu-program">
    <div class="gradient" />
    <img src={School} class="school" />
    <span class="text">
      We provide an environment where we teach students how to think rather than
      what to think
    </span>
    <div class="cards">
      <Card
        card_width="calc(100% / 1440 * 312)"
        card_height="360px"
        card_left="calc(100% / 1440 * 60)"
        card_top="128px"
        img_url={Book}
        title="Early Years"
        content="The program is for the youngest children who grow and develop very quickly"
        btn_bk_color="#DE8A2E"
        btn_text_color="#FFFFFF"
        btn_caption="Learn more"
      />

      <Card
        card_width="calc(100% / 1440 * 312)"
        card_height="360px"
        card_left="calc(100% / 1440 * 1068)"
        card_top="288px"
        img_url={Fomular}
        title="Middle Years"
        content="MYP develops empathetic and purposeful learners for a global society"
        btn_bk_color="#8E4B98"
        btn_text_color="#FFFFFF"
        btn_caption="Learn more"
      />

      <Card
        card_width="calc(100% / 1440 * 312)"
        card_height="360px"
        card_left="calc(100% / 1440 * 564)"
        card_top="570px"
        img_url={Paper}
        title="Primary Years"
        content="Develops young students as caring, active participants in a lifelong journey of learning"
        btn_bk_color="#CEDA42"
        btn_text_color="#FFFFFF"
        btn_caption="Learn more"
      />
    </div>
  </section>
  <section class="reasons">
    <div class="title-subtitle">
      <span class="title"> Reasons to join Bloomingdale </span>
      <span class="content">
        We provide an environment where we teach students how to think rather
        than what to think. We aim to provide memorable experiences that foster
        a real love of learning and personal development.
      </span>
    </div>
    <img src={ReasonImg1} class="img1" />
    <!-- <img src={ReasonImg2} class="img2"/> -->
    <span class="number">1.</span>
    <span class="scrolldown">Scroll down</span>
  </section>
  <section class="stroke2">
    <img src={Stroke2Img} class="img2" />
    <!-- <span class="text1">School for creators</span>
		<span class="text2">School for creators</span> -->
  </section>
  <section class="feedback">
    <div class="content">
      <span class="text">
        Parents' feedback about our school. We provide an environment where we
        teach students how to think rather than what to think.
      </span>
      <div class="feedbacks">
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
    <div class="stats-cards">
      <Card1
        title_color="#DE8A2E"
        title1="1/40"
        content="Schools in teh U.S. with the International Baccalaureate PYP-MYP-DP currciculum from grade PK3 through 12"
      />
      <Card1
        title_color="#8E4B98"
        title1="100"
        title2="%"
        content="Students beginning in Prekindergarten-4 take a foreing language"
      />
      <Card1
        title_color="#CEDA42"
        title1="17"
        content="Competitive sports for middle and upper school and an intramural sports program for elementary and early childhood"
      />
      <Card1
        title_color="#64A8DF"
        title1="48"
        title2="%"
        content="Full-time faculty with advanced degrees"
      />
    </div>
  </section>
  <section class="aboutus">
    <div class="title-subtitle-btn">
      <span class="title"> Reasons to join Bloomingdale </span>
      <span class="content">
        We provide an environment where we teach students how to think rather
        than what to think. We aim to provide memorable experiences that foster
        a real love of learning and personal development.
      </span>
      <Button bk_color="#FFFFFF" text_color="#DE8A2E" caption="About us" />
    </div>
    <div class="imgs">
      <img src={Rectangle1} class="img1" />
      <img src={Rectangle2} class="img2" />
      <img src={Rectangle3} class="img3" />
      <img src={Rectangle4} class="img4" />
      <img src={Rectangle5} class="img5" />
      <img src={Rectangle6} class="img6" />
    </div>
  </section>
  <section class="upevent">
    <div class="frame">
      <span class="title">Upcoming Events</span>
      <div class="frame1">
        <div class="frame2">
          <div class="frame-panel">
            <div class="content">
              <img src={Frame} class="img" />
              <div class="title-date">
                <span class="title">Sankranthi Holidays</span>
                <div class="date-frame">
                  <span>Sports</span>
                  <span style="opacity:0.5;">|</span>
                  <span>January 2022</span>
                </div>
              </div>
            </div>
            <img src={Buttonimg} class="button" />
          </div>
          <div class="frame-panel">
            <div class="content">
              <img src={Frame} class="img" />
              <div class="title-date">
                <span class="title">Open Forum- PYP-MYP</span>
                <div class="date-frame">
                  <span>Sports</span>
                  <span style="opacity:0.5;">|</span>
                  <span>January 2022</span>
                </div>
              </div>
            </div>
            <img src={Buttonimg} class="button" />
          </div>
          <div class="frame-panel">
            <div class="content">
              <img src={Frame} class="img" />
              <div class="title-date">
                <span class="title">Republic day</span>
                <div class="date-frame">
                  <span>Sports</span>
                  <span style="opacity:0.5;">|</span>
                  <span>January 2022</span>
                </div>
              </div>
            </div>
            <img src={Buttonimg} class="button" />
          </div>
        </div>
        <Button
          bk_color="#DE8A2E"
          text_color="#FFFFFF"
          caption="See all events"
        />
      </div>
    </div>
  </section>
  <section class="last-news">
    <div class="header">
      <h1>Last News</h1>
      <div class="card-control-btns">Buttons</div>
    </div>
    <div class="cards-flow">Cards</div>
    <div>
      <Button bk_color="#DE8A2E" , text_color="#fff" caption="See all news" />
    </div>

    <div class="partners">
      <h4>Trust by</h4>
      <div class="partner-cards">
        <div class="card">
          <img src={CompanyLogo1} />
        </div>
        <div class="card">
          <img src={CompanyLogo2} />
        </div>
        <div class="card">
          <img src={CompanyLogo3} />
        </div>
        <div class="card">
          <img src={CompanyLogo4} />
        </div>
        <div class="card">
          <img src={CompanyLogo5} />
        </div>
      </div>
    </div>
  </section>
  <Footer top_value="8762px" />
</section>

<style lang="scss">
  .home {
    .hero {
      position: absolute;
      width: 100%;
      height: 757px;
      left: 0px;
      top: 0px;
      background: url("../lib/images/layer1_back.png") no-repeat center center
        fixed;
      -webkit-background-size: cover;
      -moz-background-size: cover;
      -o-background-size: cover;
      background-size: cover;

      .title-img {
        /* Auto layout */
        display: flex;
        flex-direction: column;
        justify-content: flex-end;
        align-items: flex-start;
        padding: 0px;
        gap: 20px;
        isolation: isolate;

        position: absolute;
        width: calc(100% / 1440 * 533);
        height: 240px;
        left: calc(100% / 800 * 60);
        top: 239px;

        .title {
          width: 533px;
          height: 240px;

          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 80px;
          line-height: 100%;
          /* or 80px */
          color: #ffffff;

          display: flex;
          align-items: center;
          
        }
      }
    }
    .stroke-video {
      position: absolute;
      width: 100%;
      height: 1150px;
      left: 0px;
      top: 720px;

      /* Brandcolors/Mint */
      background: #a6d6c9;
      border-radius: 40px;

      overflow: hidden;

      .video {
        position: absolute;
        width: 100%;
        height: 100%;
        left: 0px;
        top: 304px;

        .play {
          position: absolute;
          width: 172px;
          height: 172px;
          left: calc(100% / 1440 * 634);
          top: calc(100% / 800 * 276);
        }

        .img {
          position: absolute;
          width: 100%;
          left: 0px;
          top: 0px;
        }
      }

      .stroke {
        position: absolute;
        width: 100%;
        height: 160px;
        // left: -calc(100% / 1440 * 544);
        top: 72px;

        .text {
          position: absolute;
          width: calc(100% / 1440 * 1400);
          height: 160px;
          left: 75%;
          top: 32px;

          /* Desktop/Running line Desktop | 160 */

          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: calc(5% * 160);
          line-height: 100%;
          /* identical to box height, or 160px */

          /* Basic & Secondary/White */

          color: #ffffff;
        }

        .img1 {
          position: absolute;
          width: calc(100% / 1440 * 260);
          left: calc(100% / 1440 * 804);
          border-radius: 20px;
        }
      }
    }

    .edu-program {
      position: absolute;
      width: 100%;
      height: 1362px;
      left: 0px;
      top: 1744px;

      /* Basic & Secondary/White */
      background: linear-gradient(
        180deg,
        #caefff 0%,
        #effffd 23.3%,
        #fff0d0 82.39%
      );
      border-radius: 40px;

      .school {
        position: absolute;
        width: 100%;
        height: calc(100% / 800 * 803);
        left: 0px;
        top: 486px;
      }

      .text {
        position: absolute;
        width: 560px;
        height: 129px;
        left: 35%;
        top: 30%;

        /* Desktop/H3 Desktop | 36 */

        font-family: "Suisse Intl";
        font-style: normal;
        font-weight: 400;
        font-size: 36px;
        line-height: 120%;
        /* or 43px */

        text-align: center;

        /* Basic & Secondary/Dark Blue */

        color: #254b6a;
      }
    }

    .reasons {
      position: absolute;
      width: 100%;
      height: 900px;
      left: 0px;
      top: 3020px;

      /* Brandcolors/Yellow */

      background: #efdb34;
      border-radius: 48px;
      overflow: hidden;

      .title-subtitle {
        /* Auto layout */

        display: flex;
        flex-direction: column;
        align-items: flex-start;
        padding: 0px;
        gap: 40px;

        position: absolute;
        width: calc(100% / 1440 * 447);
        height: calc(100% / 800 * 314);
        left: calc(100% / 1440 * 732);
        top: calc(100% / 800 * 128);

        .title {
          width: 447px;
          height: 134px;

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

        .content {
          width: 447px;
          height: 140px;

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

      .img1 {
        position: absolute;
        width: calc(100% / 1440 * 397);
        height: calc(100% / 800 * 564);
        left: calc(100% / 1440 * 223);
        top: calc(100% / 800 * 128);

        border-radius: 24px;
      }

      // .img2 {
      // 	position: absolute;
      // 	width: 312px;
      // 	height: 448px;
      // 	left: 732px;
      // 	top: 772px;

      // 	border-radius: 20px;
      // }

      .number {
        position: absolute;
        width: 99px;
        height: 160px;
        left: calc(100% / 1440 * 60);
        top: calc(100% / 800 * 128);

        /* Desktop/Running line Desktop | 160 */

        font-family: "Suisse Intl";
        font-style: normal;
        font-weight: 400;
        font-size: 160px;
        line-height: 100%;
        /* identical to box height, or 160px */

        /* Basic & Secondary/Dark Blue */

        color: #254b6a;
      }

      .scrolldown {
        position: absolute;
        width: 86px;
        height: 22px;
        left: 99px;
        top: 692px;

        /* Desktop/Body 2 Desktop | 16 */

        font-family: "Suisse Intl";
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 140%;
        /* or 22px */

        /* Basic & Secondary/Dark Blue */

        color: #254b6a;

        transform: rotate(-90deg);
      }
    }

    .stroke2 {
      position: absolute;
      width: 100%;
      height: 408px;
      left: 0px;
      top: 3840px;

      /* Brandcolors/Mint */

      background: #a6d6c9;
      border-radius: 40px;

      .img1 {
        position: absolute;
        width: 260px;
        height: 160px;
        left: 2512.78px;
        top: 75.25px;

        border-radius: 20px;
        transform: rotate(-1deg);
      }

      .img2 {
        position: absolute;
        width: calc(100% / 1440 * 260);
        left: calc(100% / 1440 * 804);
        border-radius: 10px;
      }

      .text1 {
        position: absolute;
        width: 1400px;
        height: 160px;
        left: 507px;
        top: 72px;

        /* Desktop/Running line Desktop | 160 */

        font-family: "Suisse Intl";
        font-style: normal;
        font-weight: 400;
        font-size: 160px;
        line-height: 100%;
        /* identical to box height, or 160px */

        /* Basic & Secondary/White */

        color: #ffffff;
      }

      .text2 {
        position: absolute;
        width: 1400px;
        height: 160px;
        left: -1249px;
        top: 72px;

        /* Desktop/Running line Desktop | 160 */

        font-family: "Suisse Intl";
        font-style: normal;
        font-weight: 400;
        font-size: 160px;
        line-height: 100%;
        /* identical to box height, or 160px */

        /* Basic & Secondary/White */

        color: #ffffff;
      }
    }

    .feedback {
      position: absolute;
      width: 100%;
      height: 1500px;
      left: 0px;
      top: 4144px;

      /* Basic & Secondary/White */
      background: linear-gradient(
        360deg,
        #caefff -33.82%,
        #effffd 1.46%,
        #fff0d0 90.94%
      );
      border-radius: 48px;

      .content {
        /* Auto layout */
        display: flex;
        justify-content: space-between;
        flex-direction: row;
        padding: 0px;

        left: 4.67%;
        top: 4.67%;
        z-index: 100;
        box-sizing: border-box;
        padding: 128px 60px;
        width: 100%;

        .text {
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

        .feedbacks {
          display: flex;
          flex-direction: column;
          padding: 0px;
          gap: 48px;

          width: 648px;
          height: 724px;

          /* Inside auto layout */

          flex: none;
          order: 1;
          flex-grow: 0;
        }
      }

      .stats-cards {
        /* Auto layout */

        display: flex;
        flex-direction: row;
        align-items: flex-start;
        padding: 0px;
        gap: 24px;

        position: absolute;
        width: 1320px;
        height: 312px;
        left: 61px;
        top: 980px;
      }
    }

    .aboutus {
      /* Section | About us */
      position: absolute;
      width: 100%;
      height: 900px;
      left: 0px;
      top: 5564px;

      display: flex;
      justify-content: space-between;
      box-sizing: border-box;
      padding: 0 60px;

      /* Brandcolors/Orange */

      background: #de8a2e;
      border-radius: 48px 48px 0px 0px;

      .title-subtitle-btn {
        /* Auto layout */

        display: flex;
        flex-direction: column;
        align-items: flex-start;
        padding: 209px 0;
        gap: 40px;

        width: 424px;
        height: 402px;

        .title {
          width: 424px;
          height: 134px;

          /* Desktop/H2 Desktop 56 */

          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 56px;
          line-height: 120%;
          /* or 67px */

          /* Basic & Secondary/White */

          color: #ffffff;
        }

        .content {
          width: 424px;
          height: 140px;

          /* Desktop/Body Desktop | 20 */

          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 20px;
          line-height: 140%;
          /* or 28px */

          /* Basic & Secondary/White */

          color: #ffffff;

          opacity: 0.6;
        }
      }

      .imgs {
        width: 603px;
        height: 1487px;

        .img1 {
          position: absolute;
          width: 290px;
          height: 414px;
          left: 777px;
          top: -323px;

          border-radius: 24px;
        }

        .img2 {
          position: absolute;
          width: 290px;
          height: 414px;
          left: 777px;
          top: 115px;
          border-radius: 24px;
        }

        .img3 {
          position: absolute;
          width: 290px;
          height: 414px;
          left: 1090px;
          top: 750px;
          border-radius: 24px;
        }

        .img4 {
          position: absolute;
          width: 290px;
          height: 414px;
          left: 1090px;
          top: -126px;
          border-radius: 24px;
        }

        .img5 {
          position: absolute;
          width: 290px;
          height: 414px;
          left: 1090px;
          top: 312px;
          border-radius: 24px;
        }

        .img6 {
          position: absolute;
          width: 290px;
          height: 414px;
          left: 777px;
          top: 553px;
          border-radius: 24px;
        }
      }
    }

    .upevent {
      position: absolute;
      width: 100%;
      height: 1243px;
      left: 0px;
      top: 6384px;

      /* Brandcolors/Mint */

      background: #a6d6c9;
      border-radius: 48px 48px 0px 0px;
      display: flex;
      justify-content: center;
      align-items: center;

      .frame {
        /* Auto layout */
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 0px;
        gap: 64px;

        position: absolute;
        width: 1096px;
        height: 907px;

        .title {
          width: 456px;
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

        .frame1 {
          display: flex;
          flex-direction: column;
          align-items: center;
          padding: 0px;
          gap: 64px;

          width: 1096px;
          height: 776px;

          .frame2 {
            /* Auto layout */
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            padding: 0px;
            gap: 32px;

            width: 1096px;
            height: 664px;

            .frame-panel {
              /* Auto layout */
              display: flex;
              flex-direction: row;
              align-items: flex-start;
              padding: 24px;
              gap: 305px;
              isolation: isolate;

              width: 1096px;
              height: 200px;

              background: #ffffff;
              border-radius: 24px;

              .content {
                /* Auto layout */
                display: flex;
                flex-direction: row;
                align-items: center;
                padding: 0px;
                gap: 24px;

                width: 573px;
                height: 152px;

                .img {
                  width: 220px;
                  height: 152px;

                  border-radius: 16px;
                }

                .title-date {
                  /* Auto layout */

                  display: flex;
                  flex-direction: column;
                  justify-content: space-between;
                  align-items: flex-start;
                  padding: 0px;
                  gap: 16px;

                  width: 329px;
                  height: 152px;

                  .title {
                    width: 329px;
                    height: 43px;

                    /* Desktop/H3 Desktop | 36 */

                    font-family: "Suisse Intl";
                    font-style: normal;
                    font-weight: 400;
                    font-size: 36px;
                    line-height: 120%;
                    /* or 43px */

                    /* Basic & Secondary/Dark Blue */

                    color: #254b6a;
                  }

                  .date-frame {
                    /* Auto layout */

                    display: flex;
                    flex-direction: row;
                    align-items: center;
                    padding: 0px;
                    gap: 16px;

                    width: 182px;
                    height: 28px;

                    font-family: "Suisse Intl";
                    font-style: normal;
                    font-weight: 400;
                    font-size: 16px;
                    line-height: 140%;
                    /* or 22px */

                    /* Basic & Secondary/Black */

                    color: #1e1515;

                    opacity: 0.6;
                  }
                }
              }

              .button {
                /* Auto layout */
                display: flex;
                flex-direction: row;
                padding: 0px;
                gap: 8px;

                width: 104px;
                height: 16px;
              }
            }
          }
        }
      }
    }

    .last-news {
      position: absolute;
      width: 100%;
      height: 1525px;
      left: 0px;
      top: 7547px;

      background: #ffffff;
      border-radius: 48px 48px 0px 0px;

      box-sizing: border-box;
      padding: 128px 60px;
      display: flex;
      flex-direction: column;
      gap: 30px;
      .header {
        h1 {
          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 56px;
          line-height: 120%;
          /* or 67px */

          color: #0f1121;
          float: left;
        }
        .card-control-btns {
          float: right;
        }
      }
      .cards-flow {
      }
      .partners {
        display: flex;
        flex-direction: column;
        justify-content: center;
        text-align: center;
        h4 {
          /* Desktop/Body Desktop | 20 */

          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 20px;
          line-height: 140%;
          /* identical to box height, or 28px */

          /* Basic & Secondary/Black */

          color: #1e1515;

          opacity: 0.6;
        }
        .partner-cards {
          display: flex;
          flex-direction: row;
          align-items: center;
          justify-content: space-between;
          .card {
            width: 244px;
            height: 120px;
            display: flex;
            justify-content: center;
            align-items: center;
          }
          .card:hover {
            border: 1px solid #0f1121;
          }
        }
      }
    }
  }
</style>
