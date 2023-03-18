<script>
	import Logo1 from "$lib/images/Logo1.png"
	import Burger1 from "$lib/images/Burger1.png"
	import Img1 from "$lib/images/gallery1.png"
	import Img2 from "$lib/images/gallery2.png"
	import Img3 from "$lib/images/gallery3.png"
	import Img4 from "$lib/images/gallery4.png"
	import Img5 from "$lib/images/gallery5.png"
	import Img6 from "$lib/images/gallery6.png"
	import Img7 from "$lib/images/gallery7.png"
	import Admission from "../../components/+admission.svelte";
	import Footer from "../../components/+footer.svelte";

	import { onMount } from 'svelte'
  import NavbarBlack from "../../components/Navbar/+NavbarBlack.svelte";

	onMount(() => {
		function onResize() {
			// alert(window.innerWidth);
		}
		window.addEventListener('resize', onResize);
		return () => window.removeEventListener('resize', onResize);
	});

</script>

<svelte:head>
	<title>Transport</title>
	<meta name="description" content="School Life/Transport" />
</svelte:head>



<div class="transport">
	<NavbarBlack/>
	<div class="hero">
		<div class="heared-menu">
			<img src={Logo1} class="logo">
			<div class="content">
				<div class="buttons btn">
					<button class="tour">
						Virtual Tour
					</button>
					<button class="enquiry">
						Enquiry
					</button>
				</div>
				<button class="burger"/>
			</div>
		</div>
	</div>
	<div class="gallery">
		<div class="gradient"></div>
		<div class="title-subtitle">
			<span class="title">
				Gallery
			</span>
			<span class="subtitle">
				Our School Gallery exhibits student creativity and achievements, featuring artwork, photography, music, and projects that reflect our school's culture and values.
			</span>
		</div>
		<div class="img-content">
			<img src={Img1} class="img1" />
			<img src={Img2} class="img2" />
			<img src={Img3} class="img3" />
			<img src={Img4} class="img4" />
			<img src={Img5} class="img5" />
			<img src={Img6} class="img6" />
			<img src={Img1} class="img7" />
			<img src={Img7} class="img8" />
			<img src={Img5} class="img9" />
			<img src={Img3} class="img10" />
		</div>
	</div>
  <Footer top_value="3183px" />
</div>

<style lang="scss">
	.transport {
		.hero {
			.img {
				position: absolute;
				width: 100%;
				left: 0px;
				top: 0px;
				background: linear-gradient(90deg, rgba(0, 0, 0, 0.7) -0.45%, rgba(0, 0, 0, 0.28) 100%);
			}
	
			.logo {
				width: calc(100% / 1440 * 206);
			}
	
			.button {
				box-sizing: border-box;
			}
	
			.heared-menu {
				display: flex;
				flex-direction: row;
				align-items: center;
				padding: calc(100% / 800 * 24) calc(100% / 1440 * 60);
				gap: calc(100% / 1440 * 804);

				position: absolute;
				width: 91%;
				height: calc(100% / 800 * 88);
				left: 0px;
				top: 0px;

				.content {
					display: flex;
					flex-direction: row;
					justify-content: center;
					align-items: center;
					padding: 0px;
					gap: calc(100% / 1440 * 24);

					width: calc(100% / 1440 * 310);
					height: calc(100% / 800 * 40);

					.buttons {
						display: flex;
						flex-direction: row;
						justify-content: center;
						align-items: center;
						padding: 0px;
						gap: calc(100% / 800 * 8);

						width: 246px;
						height: 40px;

						.tour {
							display: flex;
							flex-direction: row;
							justify-content: center;
							align-items: center;
							padding: 12px 24px;
							gap: 10px;
							width: 133px;
							height: 40px;
							background: transparent;
							border: none;
							color: #000000;
						}

						.enquiry {
							display: flex;
							flex-direction: row;
							justify-content: center;
							align-items: center;
							padding: 12px 24px;
							gap: 10px;
							width: 105px;
							height: 40px;
							background: #FFFFFF;
							border-radius: 100px;
							border: none;
						}
					}

					.burger {
						width: 40px;
						height: 40px;
						border: none;
						background: transparent;
						background-image: url("../../lib/images/Burger1.png");
					}
				}
			}
	
			.title-subtitle {
				display: flex;
				flex-direction: column;
				justify-content: center;
				align-items: flex-start;
				padding: 0px;
				gap: calc(100% / 1440 * 40);
		
				position: absolute;
				width: calc(100% / 1440 * 470);
				height: calc(100% / 800 * 191);
				left: calc(100% / 1440 * 60);
				top: calc(100% / 800 * 401);
		
				.title {
					width: 245px;
					height: 67px;
					font-family: 'Suisse Intl';
					font-style: normal;
					font-weight: 400;
					font-size: 56px;
					line-height: 120%;		
					color: #FFFFFF;
				}
		
				.subtitle {
					width: 470px;
					height: 84px;
					font-family: 'Suisse Intl';
					font-style: normal;
					font-weight: 400;
					font-size: 20px;
					line-height: 140%;
					color: #FFFFFF;
				}
			}
		}

		.gallery {
			position: absolute;
			width: 100%;
			height: calc(100% / 800 * 3565);
			left: 0px;
			top: 0px;
			border-radius: 0px;

			.title-subtitle {
				display: flex;
				flex-direction: column;
				align-items: center;
				padding: 0px;
				gap: 40px;

				position: absolute;
				width: calc(100% / 1440 * 552);
				height: 191px;
				left: calc(100% / 1440 * 444);
				top: 216px;

				.title {
					width: 552px;
					height: 67px;

					/* Desktop/H2 Desktop 56 */

					font-family: 'Suisse Intl';
					font-style: normal;
					font-weight: 400;
					font-size: 56px;
					line-height: 120%;
					/* or 67px */

					text-align: center;

					/* Basic & Secondary/Black */

					color: #1E1515;
				}

				.subtitle {
					width: 552px;
					height: 84px;

					/* Desktop/Body Desktop | 20 */

					font-family: 'Suisse Intl';
					font-style: normal;
					font-weight: 400;
					font-size: 20px;
					line-height: 140%;
					/* or 28px */

					text-align: center;

					/* Basic & Secondary/Black */

					color: #1E1515;

					opacity: 0.6;
				}
			}

			.img-content {
				position: absolute;
				width: calc(100% / 1440 * 628);
				height: calc(100% / 800 * 400);
				left: calc(100% / 1440 * 80);
				top: 0px;

				background: url(image.png);
				border-radius: 24px;

				.img1 {
					position: absolute;
					width: 100%;
					left: 1.5%;
					top: 24%;

					border-radius: 24px;
				}

				.img2 {
					position: absolute;
					width: 100%;
					left: 103.5%;
					top: 24%;

					border-radius: 24px;
				}

				.img3 {
					position: absolute;
					width: 120%;
					left: 1.5%;
					top: 50%;

					border-radius: 24px;
				}

				.img4 {
					position: absolute;
					width: 80%;
					height: 26%;
					left: 123.5%;
					top: 50%;

					border-radius: 24px;
				}

				.img5 {
					position: absolute;
					width: 80%;
					height: 26%;
					left: 123.5%;
					top: 77%;

					border-radius: 24px;
				}

				.img6 {
					position: absolute;
					width: 100%;
					left: 1.5%;
					top: 104%;

					border-radius: 24px;
				}

				.img7 {
					position: absolute;
					width: 100%;
					left: 103.5%;
					top: 104%;

					border-radius: 24px;
				}

				.img8 {
					position: absolute;
					width: 80%;
					height: 26%;
					left: 1.5%;
					top: 130%;

					border-radius: 24px;	
				}

				.img9 {
					position: absolute;
					width: 80%;
					height: 26%;
					left: 1.5%;
					top: 157%;

					border-radius: 24px;
				}

				.img10 {
					position: absolute;
					width: 120%;
					left: 83.5%;
					top: 130%;

					border-radius: 24px;
				}
			}

			.gradient {
				position: absolute;
				width: 100%;
				height: calc(100% / 800 * 3967);
				left: 0px;
				top: 0px;

				/* Basic & Secondary/Gradient Blue & Orange */

				background: linear-gradient(180deg, #CAEFFF 0%, #EFFFFD 23.3%, #FFF0D0 82.39%);
			}
		}
	}
</style>