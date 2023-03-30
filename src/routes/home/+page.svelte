<script>
  //
  import { onMount, afterUpdate } from "svelte";
  import gsap from "gsap";
  import { fade, scale } from "svelte/transition";
  import ScrollTrigger from "gsap/ScrollTrigger";
  import ScrollMagic from "scrollmagic";
  import Scrollbar from "smooth-scrollbar";
  import { TimelineMax } from "gsap/gsap-core";

  // image import
  import Student1 from "$lib/images/student1.png";
  import Student2 from "$lib/images/student2.png";
  import StrokeInnerImg1 from "$lib/images/strokeInnerImg1.png";
  import Videobg from "$lib/images/video.png";
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
  import CompanyLogo1 from "$lib/images/Microsoft-Showcase-School 1.png";
  import CompanyLogo2 from "$lib/images/nba-seeklogo.com 1.png";
  import CompanyLogo3 from "$lib/images/Frame 1000004283.png";
  import CompanyLogo4 from "$lib/images/la-liga-seeklogo.com 1.png";
  import CompanyLogo5 from "$lib/images/image 1554.png";
  import Frame from "$lib/images/frame.png";
  import Buttonimg from "$lib/images/Button.png";

  //Component Import
  import Navbar from "../../components/Navbar/+navbar.svelte";
  import Card from "../../components/Cards/Card.svelte";
  import Card1 from "../../components/Cards/Card1.svelte";
  import Feedback from "../../components/Cards/Feedback.svelte";
  import Button from "../../components/+button.svelte";
  import Footer from "../../components/+footer.svelte";

  onMount(() => {
    gsap.registerPlugin(ScrollTrigger);
    //hero section animation
    gsap.from(
      ".inner",
      1,
      {
        yPercent: 100,
        duration:2,
        delay:1,
        ease: "Back.easeOut",
      }
    );
    //stroke section animation
    gsap.utils.toArray(".stroke-text").forEach((stroke, index) => {
      const w = stroke.querySelector(".wrapper");
      const [x, xEnd] =
        index % 2
          ? ["100%", (w.scrollWidth - stroke.offsetWidth) * -1]
          : [w.scrollWidth * -1, 0];
      let strokeTL = gsap.timeline({
        scrollTrigger: {
          trigger: ".stroke",
          start: "top center",
          end: "bottom bottom",
          scrub: true,
          pin: false,
          anticipatePin: 1,
        },
      });
      strokeTL.fromTo(
        w,
        { x },
        {
          x: xEnd*2,

          duration: 0.8,
        }
      );
    });
    //video section animation
    let timeline = gsap.timeline({
      scrollTrigger: {
        trigger: ".video",
        start: "bottom bottom",
        end: "bottom bottom",
        scrub: true,
        pin: false,
        anticipatePin: 1,
      },
    });
    timeline
      .add("start")
      .to(".mask", { duration: 3, scale: 15, ease: "Back.easeOut"}, "start")
      .to(".mask", { duration: 2, rotate: -90 }, "start");

    //education section animation
    let tl = gsap.timeline({
      scrollTrigger: {
        trigger: ".edu-program",
        start: "top center",
        end: "bottom bottom",
        scrub: true,
        pin: false,
        anticipatePin: 1,
      },
    });
    tl.fromTo(
      ".edu-program p",
      {
        opacity: 0,
        y: "100%",
      },
      {
        duration: 3,
        opacity: 2,
        y: -200,
        delay: 0.5,
      }
    )
    //resons animation
    //about us animation
    gsap.utils.toArray(".image-list").forEach((section, index) => {
      const w = section.querySelector(".wrapper");
      const [y, xEnd] =
        index % 2
          ? ["100%", (w.scrollHeight - section.offsetHeight) * -1]
          : [w.scrollHeight * -1, 0];
      gsap.fromTo(
        w,
        { y },
        {
          y: xEnd,
          scrollTrigger: {
            trigger: ".aboutus",
            scrub: 0.5,
          },
          duration: 0.8,
        }
      );
    });
  });
</script>

<svelte:head>
  <title>Homepage</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>

<div class="home">
  <Navbar />
  <section class="hero">
    <div class="title-img">
      <div class="outer">
        <div class="inner">The <span style="color: #DE8A2E;"> #1</span></div>
      </div>
      <div class="outer">
        <div class="inner">
          <img src={Student1} class="img1" alt="student1" />
          <img src={Student2} class="img2" alt="student2" />
          <span class="txt">&nbsp;School for</span>
        </div>
      </div>
      <div class="outer"><div class="inner">performers</div></div>
    </div>
  </section>
  <section class="stroke first">
    <!-- svelte-ignore a11y-img-redundant-alt -->
    <div class="stroke-text">
      <p class="wrapper">
        School for creators <span
          ><img
            src={StrokeInnerImg1}
            class="stroke-inner-img"
            alt="stroke inner image"
          /></span
        > School for creators
      </p>
    </div>
    <!-- svelte-ignore a11y-img-redundant-alt -->
    <div class="stroke-text">
      <p class="wrapper">
        School for creators <span
          ><img
            src={StrokeInnerImg1}
            class="stroke-inner-img"
            alt="stroke inner image"
          /></span
        > School for creators
      </p>
    </div>
  </section>
  <section class="video">
    <div class="mask" />
    <div class="video-item" />
  </section>
  <section class="edu-program">
    <p class="title">
      We provide an environment where we teach students how to think rather than
      what to think
    </p>
    <div class="cards">
      <Card
        card_left="60px"
        card_top="128px"
        img_url={Book}
        title="Early Years"
        content="The program is for the youngest children who grow and develop very quickly"
        btn_bk_color="#DE8A2E"
        btn_text_color="#FFFFFF"
        btn_caption="Learn more"
      />

      <Card
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
    <div class="content">
      <div class="image-view">
        <div class="title">
          <p class="number">1.</p>
          <p class="scrolldown">Scroll down</p>
        </div>
        <div class="images">
          <!-- svelte-ignore a11y-missing-attribute -->
          <img src={ReasonImg1} class="img1" />
        </div>
      </div>
      <div class="title-subtitle">
        <h1 class="title">Reasons to join Bloomingdale</h1>
        <p class="content">
          We provide an environment where we teach students how to think rather
          than what to think. We aim to provide memorable experiences that
          foster a real love of learning and personal development.
        </p>
      </div>
    </div>
  </section>
  <section class="stroke second">
    <!-- svelte-ignore a11y-img-redundant-alt -->
    <div class="stroke-text">
      <p class="wrapper">
        School for creators <span
          ><img
            src={Stroke2Img}
            class="stroke-inner-img"
            alt="stroke inner image"
          /></span
        > School for creators
      </p>
    </div>
    <!-- svelte-ignore a11y-img-redundant-alt -->
    <div class="stroke-text">
      <p class="wrapper">
        School for creators <span
          ><img
            src={Stroke2Img}
            class="stroke-inner-img"
            alt="stroke inner image"
          /></span
        > School for creators
      </p>
    </div>
  </section>
  <section class="feedback">
    <div class="feedback-content">
      <p class="text">
        Parents' feedback about our school. We provide an environment where we
        teach students how to think rather than what to think.
      </p>
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
    <!-- <div class="stats-cards">
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
    </div> -->
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
      <div class="image-list">
        <ul class="wrapper">
          <li><img src={Rectangle1} alt="image1" /></li>
          <li><img src={Rectangle2} alt="image2" /></li>
          <li><img src={Rectangle3} alt="image3" /></li>
          <li><img src={Rectangle4} alt="image4" /></li>
          <li><img src={Rectangle5} alt="image5" /></li>
          <li><img src={Rectangle6} alt="image6" /></li>
        </ul>
      </div>
      <div class="image-list">
        <ul class="wrapper">
          <li><img src={Rectangle1} alt="image1" /></li>
          <li><img src={Rectangle2} alt="image2" /></li>
          <li><img src={Rectangle3} alt="image3" /></li>
          <li><img src={Rectangle4} alt="image4" /></li>
          <li><img src={Rectangle5} alt="image5" /></li>
          <li><img src={Rectangle6} alt="image6" /></li>
        </ul>
      </div>
    </div>
  </section>
  <section class="upevent">
    <div class="frame">
      <span class="title">Upcoming Events</span>
      <div class="frame1">
        <div class="frame2">
          <div class="frame-panel">
            <div class="content">
              <img src={Frame} class="img" alt="frame" />
              <div class="title-date">
                <span class="title">Sankranthi Holidays</span>
                <div class="date-frame">
                  <span>Sports</span>
                  <span style="opacity:0.5;">|</span>
                  <span>January 2022</span>
                </div>
              </div>
            </div>
            <img src={Buttonimg} class="button" alt="buttong" />
          </div>
          <div class="frame-panel">
            <div class="content">
              <img src={Frame} class="img" alt="button" />
              <div class="title-date">
                <span class="title">Open Forum- PYP-MYP</span>
                <div class="date-frame">
                  <span>Sports</span>
                  <span style="opacity:0.5;">|</span>
                  <span>January 2022</span>
                </div>
              </div>
            </div>
            <img src={Buttonimg} class="button" alt="button" />
          </div>
          <div class="frame-panel">
            <div class="content">
              <img src={Frame} class="img" alt="frame" />
              <div class="title-date">
                <span class="title">Republic day</span>
                <div class="date-frame">
                  <span>Sports</span>
                  <span style="opacity:0.5;">|</span>
                  <span>January 2022</span>
                </div>
              </div>
            </div>
            <img src={Buttonimg} class="button" alt="button" />
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
      <div class="card-control-btns">
        <button class="prev">&#60;</button>
        <button class="next">&#62;</button>
      </div>
    </div>
    <div class="cards-flow">
      <div class="last-news-card">
        <img src={Rectangle5} alt="last news card" />
        <p>5th Annual Sports Meet</p>
        <a href="#">Read all &#x2B95</a>
      </div>
      <div class="last-news-card">
        <img src={Rectangle5} alt="last news card" />
        <p>5th Annual Sports Meet</p>
        <a href="#">Read all &#x2B95</a>
      </div>
      <div class="last-news-card">
        <img src={Rectangle5} alt="last news card" />
        <p>5th Annual Sports Meet</p>
        <a href="#">Read all &#x2B95</a>
      </div>
      <div class="last-news-card">
        <img src={Rectangle5} alt="last news card" />
        <p>5th Annual Sports Meet</p>
        <a href="#">Read all &#x2B95</a>
      </div>
      <div class="last-news-card">
        <img src={Rectangle5} alt="last news card" />
        <p>5th Annual Sports Meet</p>
        <a href="#">Read all &#x2B95</a>
      </div>
      <div class="last-news-card">
        <img src={Rectangle5} alt="last news card" />
        <p>5th Annual Sports Meet</p>
        <a href="#">Read all &#x2B95</a>
      </div>
      <div class="last-news-card">
        <img src={Rectangle5} alt="last news card" />
        <p>5th Annual Sports Meet</p>
        <a href="#">Read all &#x2B95</a>
      </div>
      <div class="last-news-card">
        <img src={Rectangle5} alt="last news card" />
        <p>5th Annual Sports Meet</p>
        <a href="#">Read all &#x2B95</a>
      </div>
      <div class="last-news-card">
        <img src={Rectangle5} alt="last news card" />
        <p>5th Annual Sports Meet</p>
        <a href="#">Read all &#x2B95</a>
      </div>
      <div class="last-news-card">
        <img src={Rectangle5} alt="last news card" />
        <p>5th Annual Sports Meet</p>
        <a href="#">Read all &#x2B95</a>
      </div>
      <div class="last-news-card">
        <img src={Rectangle5} alt="last news card" />
        <p>5th Annual Sports Meet</p>
        <a href="#">Read all &#x2B95</a>
      </div>
    </div>
    <div>
      <Button bk_color="#DE8A2E" text_color="#fff" caption="See all news" />
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
  <Footer />
</div>

<style lang="scss">
  :global(body) {
    margin: 0;
  }

  :global(section) {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
  }

  .home {
    section {
      display: flex;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
    }
    .hero {
      background: url("../../lib/images/layer1_bg.png") no-repeat center center;
      -webkit-background-size: cover;
      -moz-background-size: cover;
      -o-background-size: cover;
      background-size: cover;

      justify-content: left;

      .title-img {
        /* Auto layout */
        display: flex;
        flex-direction: column;
        gap: 20px;
        isolation: isolate;
        margin-left: 60px;
        .outer {
          float: left;
          overflow: hidden;
          .inner {
            position: relative;
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
    }

    .first {
      flex-direction: column;
      background: #a6d6c9;
      overflow: hidden;
      gap: unset;

      .stroke-text .wrapper {
        font-family: "Suisse Intl";
        font-style: to-upper-case($string: "");
        font-weight: 400;
        font-size: 120px;
        line-height: 100%;
        color: #ffffff;
        rotate: -3deg;
        width: max-content;
        margin-bottom: unset;
        text-transform: uppercase;
      }
      .stroke-text .wrapper img {
        vertical-align: middle;
      }
    }

    .video {
      overflow: hidden;

      background: url("../../lib/images/video.png") no-repeat center center;
      -webkit-background-size: cover;
      -moz-background-size: cover;
      -o-background-size: cover;
      background-size: cover;

      .mask {
        width: 100%;
        height: 100%;
        background: #fff;
        -webkit-background-size: cover;
        -moz-background-size: cover;
        -o-background-size: cover;
        background-size: cover;
        mask-image: url("../../lib/images/video-mask.png");
        -webkit-mask-image: url("../../lib/images/video-mask.png");
        mask-repeat: no-repeat;
        -webkit-mask-repeat: no-repeat;
        mask-position: center;
        -webkit-mask-position: center;
        mask-size: 100%;
        -webkit-mask-size: 100%;
      }

      .video-item {
        .img {
          width: 100%;
        }
      }
    }

    .edu-program {
      position: relative;
      overflow: hidden;

      background: linear-gradient(
        180deg,
        #caefff 0%,
        #effffd 23.3%,
        #fff0d0 82.39%
      );

      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      .title {
        /* Desktop/H3 Desktop | 36 */
        width: 560px;
        height: 129px;

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
      /* Brandcolors/Yellow */

      background: #efdb34;
      overflow: hidden;
      box-sizing: border-box;
      padding: 128px 60px;

      .content {
        display: flex;
        width: 100%;
        .image-view {
          width: 50%;

          display: flex;
          flex-direction: row;
          gap: 64px;

          .title {
            display: flex;
            flex-direction: column;
            .number {
              font-family: "Suisse Intl";
              font-style: normal;
              font-weight: 400;
              font-size: 160px;
              line-height: 100%;
              color: #254b6a;
              margin: 0;
            }

            .scrolldown {
              font-family: "Suisse Intl";
              font-style: normal;
              font-weight: 400;
              font-size: 16px;
              line-height: 140%;
              color: #254b6a;
              transform: rotate(-90deg);
            }
          }
          .images {
            img {
              border-radius: 24px;
            }
          }
        }

        .title-subtitle {
          width: 50%;
          .title {
            width: 447px;
            height: 134px;

            font-family: "Suisse Intl";
            font-style: normal;
            font-weight: 400;
            font-size: 56px;
            line-height: 120%;

            color: #254b6a;
          }

          .content {
            width: 447px;
            height: 140px;

            font-family: "Suisse Intl";
            font-style: normal;
            font-weight: 400;
            font-size: 20px;
            line-height: 140%;
            color: #254b6a;
          }
        }
      }

      // .img2 {
      // 	position: absolute;
      // 	width: 312px;
      // 	height: 448px;
      // 	left: 732px;
      // 	top: 772px;

      // 	border-radius: 20px;
      // }
    }

    .second {
      background: #a6d6c9;
      overflow: hidden;
      gap: unset;
      flex-direction: column;

      .stroke-text .wrapper {
        font-family: "Suisse Intl";
        font-style: to-upper-case($string: "");
        font-weight: 400;
        font-size: 120px;
        line-height: 100%;
        color: #ffffff;
        rotate: -3deg;
        width: max-content;
        margin-bottom: unset;
        text-transform: uppercase;
      }
      .stroke-text .wrapper img {
        vertical-align: middle;
      }
    }

    .feedback {
      /* Basic & Secondary/White */
      background: linear-gradient(
        360deg,
        #caefff -33.82%,
        #effffd 1.46%,
        #fff0d0 90.94%
      );

      box-sizing: border-box;
      padding: 128px 60px;

      .feedback-content {
        /* Auto layout */
        display: flex;
        justify-content: space-between;
        flex-direction: row;
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

        .feedback-cards {
          width: 648px;
          height: 724px;
        }
      }

      .stats-cards {
        /* Auto layout */

        display: flex;
        flex-direction: row;
        align-items: flex-start;
        padding: 0px;
        gap: 24px;
      }
    }

    .aboutus {
      box-sizing: border-box;

      padding: 120px 60px;

      /* Brandcolors/Orange */

      background: #de8a2e;
      display: flex;
      justify-content: space-between;
      flex-direction: row;

      overflow: hidden;
      .title-subtitle-btn {
        /* Auto layout */

        display: flex;
        flex-direction: column;
        align-items: flex-start;
        gap: 40px;

        width: 424px;
        height: 402px;

        float: left;

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
        display: flex;
        flex-direction: row;
        .image-list {
          ul {
            list-style: none;
          }
        }
      }
    }

    .upevent {
      background: #a6d6c9;

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
      background: #ffffff;
      border-radius: 48px 48px 0px 0px;

      box-sizing: border-box;
      padding: 128px 60px;
      display: flex;
      flex-direction: column;
      gap: 30px;

      overflow: hidden;
      .header {
        display: flex;
        align-items: end;
        justify-content: space-between;

        h1 {
          font-family: "Suisse Intl";
          font-style: normal;
          font-weight: 400;
          font-size: 56px;
          line-height: 120%;
          /* or 67px */

          color: #0f1121;
          margin: 0;
        }
        .card-control-btns {
          button {
            width: 30px;
            height: 30px;
            font-size: 24px;
            border: none;
            background-color: #fff;
          }
        }
      }
      .cards-flow {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
        gap: 2%;

        .last-news-card {
          img {
            width: 424px;
            height: 424px;
          }
          p {
            font-family: "Suisse Intl Bold";
            font-style: normal;
            font-size: 20px;
            line-height: 140%;
            /* identical to box height, or 28px */

            color: #1e1515;
          }
          a {
            font-family: "Suisse Intl";
            font-style: normal;
            font-weight: 500;
            font-size: 16px;
            line-height: 100%;
            /* identical to box height, or 16px */

            /* Basic & Secondary/Black */

            color: #1e1515;
            text-decoration: none;
          }
        }
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
