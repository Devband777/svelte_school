<script>
  import Footer from "../../components/+footer.svelte";
  import Feedback from "../../components/Cards/Feedback.svelte";
  import Collapse from "../../components/+Collapse.svelte";
  import Admission from "../../components/+admission.svelte";
  import Navbar from "../../components/Navbar/+navbar.svelte";

  let collapse_content_1 =
    "<p>Learning as a holistic process, addressing physical, emotional, social and cognitive dimensions</p>" +
    "<p>Building readiness for Primary Years Programme</p>" +
    "<p>Building readiness for Primary Years Programme</p>";
</script>

<svelte:head>
  <title>Primary Years</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>
<div class="diploma">
  <Navbar/>
  <section class="hero">
    <div class="intro-text">
      <div class="title">Diploma Programme</div>
      <div class="desc">
        Grades 11 and 12 at ois follow the most challenging and comprehensive
        curriculum - the international baccalaureate diploma programme (IBDP).
        The IB diploma is globally recognized as a highly valued university
        entry qualification.
      </div>
    </div>
  </section>
  <section class="intro">
    <div class="content">
      <div class="title">Diploma Programme at Bloomingdale</div>
      <div class="paragraph">
        The IB Diploma Programme is an exciting, holistic programme that fosters
        the intellectual, social, emotional, and physical well-being of students
        in Grades 11 & 12. It aims to create learning experiences that are a
        combination of rigorous academics, creative work, collaboration, and
        social interactions. The DP curriculum prepares students for success at
        university and life beyond by providing them with the necessary skills
        and values to overcome challenges in today’s complex, dynamic and
        interconnected world.<br /><br /> Grade 11 students who opt to enrol as
        IB Diploma Candidates must meet the following requirements of the IB
        Diploma Programme: A student selects a total of 6 IBDP subjects: Studies
        in Language and Literature (Group 1), Language Acquisition (Group 2),
        Individuals and Societies (Group 3), Sciences (Group 4), Mathematics
        (Group 5), and the Arts (Group 6). Alternatively, students may choose to
        take an additional subject from Group 2, 3 or Group 4 in place of a
        subject from Group 6. Three of the above-mentioned 6 subjects will be
        taken at the Higher Level (HL), and 3 will be taken at the Standard
        Level (SL). Students also work on the 3 core components: Theory of
        Knowledge (ToK), Extended Essay (EE), and Creativity, Activity, Service
        (CAS).<br /><br /> All OlS students are eligible to receive the OIS High
        School Diploma (Grades 9 - 12), provided they meet the OIS graduation requirements.
        Oberoi International School is accredited by both the Council of International
        Schools (CIS) and the New England Association of Schools and Colleges (NEASC).
        Therefore, colleges and universities recognize the OIS High School Diploma.
      </div>
    </div>
  </section>
  <section class="point">
    <div>
      <div class="title">DP Subject offerings</div>
      <div class="subtitle">
        OIS students are prepared to be global leaders and decision-makers of
        tomorrow.
      </div>
    </div>
    <div class="content">
      <div class="left">
        <Collapse caption="Group 1" content={collapse_content_1} />
        <Collapse caption="Group 2" content={collapse_content_1} />
        <Collapse caption="Group 3" content={collapse_content_1} />
        <Collapse caption="Group 4" content={collapse_content_1} />
        <Collapse caption="Group 5" content={collapse_content_1} />
        <Collapse caption="Group 6" content={collapse_content_1} />
        <Collapse caption="Group 7" content={collapse_content_1} />
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
  
  <Admission top_value="4094px" />
  <Footer top_value="4700px"/>
</div>

<style lang="scss">
  .diploma {
    
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

        width: 1320px;
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
    .point {
      position: absolute;
      width: 100%;
      height: 1462px;
      left: 0px;
      top: 1732px;

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
      top: 3114px;

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
      top: 4094px;

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
