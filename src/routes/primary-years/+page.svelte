<script>
  import Logo from "$lib/images/Logo.png";
  import Footer from "../../components/+footer.svelte";
  import Button from "../../components/+button.svelte";
  import Feedback from "../../components/Cards/Feedback.svelte";
  import Collapse from "../../components/+Collapse.svelte";
  import ArrowDown from "$lib/images/arrow-down.png"
	import Arrow from "$lib/images/arrow.png"
  import Admission from "../../components/+admission.svelte";
  import Navbar from "../../components/Navbar/+navbar.svelte";

  let collapse_content_1 =
    "<h4>1. Create a Lifelong Love for Learning</h4> " +
    "<p>By inculcating in its learners, a desire to learn, a natural curiosity about the world, and develop the skills they need to ask questions and seek answers through research and inquiry.</p>" +
    "<h4>2. Build Responsible Citizens – Who Share and Care</h4> " +
    "<p>By developing an understanding of social problems so that students can emerge as caring and responsible citizens.</p>" +
    "<h4>3. Equip Students with Critical 21st Century Skills</h4> " +
    "<p>By teaching them the tools for success in work and life – thinking, research, communication, self-management and social skills.</p>" +
    "<h4>4. Instil Global Cultural Perspectives</h4> " +
    "<p>By developing an appreciation and understanding of one’s own, as well as other cultures to become internationally-minded citizens.</p>" +
    "<h4>5. Encourage a Proactive Approach</h4> " +
    "<p>By enabling children to develop their voice and take charge of their own learning and development.</p>";
</script>

<svelte:head>
  <title>Primary Years</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>
<div class="primary-years">
  <Navbar/>
  <section class="hero">
    <div class="intro-text">
      <div class="title">Primary Years Programme</div>
      <div class="desc">
        The IB Primary Years Programme (PYP) for children aged 3 – 12 nurtures
        and develops young students as caring, active participants in a lifelong
        journey of learning
      </div>
    </div>
  </section>
  <section class="intro">
    <div class="content">
      <div class="title">Primary Years Programme at Bloomingdale</div>
      <div class="paragraph">
        The IB Primary Years Programme (PYP) for children aged 3 – 12 nurtures
        and develops young students as caring, active participants in a lifelong
        journey of learning.Through its inquiry-led, trans-disciplinary
        framework, the PYP challenges students to think for themselves and take
        responsibility for their learning as they explore local and global
        issues and opportunities in real-life contexts. The PYP Playlist is an
        introduction for parents and teachers who are new to the Primary Years
        Programme. It contains a wide range of e-learning resources to help
        everyone in the learning community develop a deeper understanding of the
        programme, and become more active in supporting student learning. For
        more information: www.ibo.org
      </div>
    </div>
  </section>
  <section class="point">
    <div>
      <div class="title">Learners in the BIS</div>
      <div class="subtitle">The Primary Years Programme at BIS aims to</div>
    </div>
    <div class="content">
      <div class="left">
        <Collapse caption="Learning aims" content={collapse_content_1} />
        <Collapse caption="Learning and Teaching"/>
        <Collapse caption="Learning Community"/>
      </div>
      <div class="right" />
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
  <Admission top_value="3729px" />

  <Footer top_value="4335px"/>
</div>

<style lang="scss">
  .primary-years {
    
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
        url("../../lib/images/primary-years.png");
      .intro-text {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        padding: 0px;
        gap: 40px;

        position: absolute;
        width: 536px;
        height: 286px;
        left: 80px;
        top: 306px;

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
      gap: 10px;

      position: absolute;
      width: 100%;
      height: 672px;
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
          width: 403px;
          height: 129px;
          /* Inside auto layout */
          flex: none;
          order: 0;
          flex-grow: 0;
        }

        .paragraph {
          width: 648px;
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
    .point {
      position: absolute;
      width: 100%;
      height: 1515px;
      left: 0px;
      top: 1312px;

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
        top: 235px;
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
        top: 351px;
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
      top: 2747px;

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
      top: 3729px;

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
						color: #FFFFFF;

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
						background: #FFFFFF;
						border-radius: 100px;
						border: none;
						
						/* Desktop/btn1 Desktop | 16 */
						font-family: 'Suisse Intl';
						font-style: normal;
						font-weight: 500;
						font-size: 16px;
						line-height: 100%;
						/* identical to box height, or 16px */

						/* Brandcolors/Orange */
						color: #DE8A2E;

						.arrow {
							width: 32px;
							height: 32px;
						}
					}
				}
    }
  }
</style>
