<script>
	import sports_hero from "$lib/images/Sports_logo.png";
	import logo from "$lib/images/Logo.png";
	import burger from "$lib/images/Burger.png";
	import reason_image1 from "$lib/images/reason_image1.png";
	import reason_image2 from "$lib/images/reason_image2.png";
</script>
<svelte:head>
	<title>sports</title>
	<meta name="description" content="Sports" />
</svelte:head>
	<div class="sports">
		<div class="hero">
			<img src={(sports_hero)} alt="">
			<div class="heared_menu">
				<div class="logo">
					<img src={(logo)} alt="">
				</div>
				<div class="content">
					<div class="button_group">
						<div class="button_one btn" style="background-color: transparents;">Virtual Tour</div>
						<div class="button_two" style="background-color: white;"><span class="btn">Enquiry</span></div>
					</div>
					<div class="burger" style="background-color: transparents;"><img src={(burger)} alt=""></div>
				</div>
			</div>
			<div class="title_subtitle">
				<h2>Sports</h2>
				<span class="subtitle bodyR">There are a variety of clubs for students to join throughout the year. Starting from Grade 1 children get to pick sports of their choice.</span>
			</div>
		</div>
		<div class="intro gradient">
			<div class="content">
				<h3 style="float:left; margin-top:0;">School Sports Activities</h3>
				<span class="paragraph">There are a variety of clubs for students to join throughout the year. Starting from Grade 1 children get to pick sports of their choice.</span>
			</div>
		</div>
		<div class="reasons yellow">
			<h1>1.</h1>
			<div class="reason_image1">
				<img src={(reason_image1)} alt="">
			</div>
			<div class="title_subtitle">
				<h2>Football (LaLiga)</h2>
				<span class="subtitle bodyR">LaLiga Football Schools has been set-up to train the students and teach them to play the ‘Spanish Way’. Through this partnership, students will get access to Spanish training methodologies which have been specially designed by LaLiga Football Schools’ Global Technical Director and his team, and tailor-made to suit the Indian students.</span>
			</div>
			<span class="scroll body2R">Scroll Down</span>
			<div class="reason_image2">
				<img src={(reason_image2)} alt="">
			</div>
		</div>
	</div>
<style lang="scss">
	.sports {
		.hero {
			width: 1440px;
			height: 800px;
			left: 0px;
			top: 0px;
			z-index: -10;
			position: relative;
			.heared_menu {
				align-items: center;
				position: absolute;
				padding: 24px 60px;
				gap: 804px;
				width: 100%;
				height: 11%;
				left: 0px;
				top: 0px;
				.logo {
					position: absolute;
					left: 60px;
					top: 28px;
				}
				.content {
					position:absolute;
					right: 60px;
					top:28px;
					.button_group{
						.button_one{
							color: #fff;
							position:absolute;
							width: 133px;
							height: 40px;
							border-radius: 100px;
							right: 286px;
							padding: 12px;
							}
						.button_two{
							position:absolute;
							text-align: center;
							width: 100px;
							height: 40px;
							border-radius: 100px;
							right: 200px;
							.btn {
								position: relative;
								top: 10px;
							}
						}
					}
					.burger {
						position:absolute;
						right: 130px;
					}
				}
			}
			.title_subtitle {
				position: absolute;
				width: 470px;
				height: 290px;
				bottom : 200px;
				left: 60px;
				h2 {					
					color: #fff;
				}
				.subtitle {
					position: absolute;
					bottom: 0px;					
					color: #fff;
				}
			}
		}
		.intro {
			width: 1440px;
			height: 420px;
			left: 0px;
			margin-top: -80px;
			gap: 10px;
			border-radius: 48px 48px 0px 0px;
			position: relative;
			z-index: -9;
			.content {
				position: absolute;
				padding: 0px;
				gap: 64px;
				width: 1320px;
				height: 84px;
				top:128px;
				left:64px;
				.paragraph {
					position: absolute;
					opacity: 0.6;
					right: 60px;
					width: 648px;
					float: right;
				}
			}
		}
		.reasons {
			width: 1440px;
			height: 900px;
			left: 0px;
			margin-top: -80px;
			border-radius: 48px;
			position: relative;
			z-index: -7;
			h1 {
				position: absolute;
				top: 128px;
				left: 60px;
				font-size: 160px;
				margin-top: 0;
				color: #254B6A;
			}
			.reason_image1 {
				position: absolute;
				top: 128px;
				left: 223px;
			}
			.reason_image2 {
				position: absolute;
				top: 772px;
				left: 732px;
			}
			.title_subtitle {
				position: absolute;
				top: 128px;
				left: 732px;
				width: 536px;
				height: 303px;
				h2 {
					color: #254B6A;
					margin-top: 0;
				}
				.subtitle {
					color: #254B6A;
				}
			}
			.scroll {
				position: absolute;
				top: 606px;
				left: 100px;
				color: #254B6A;
				transform: rotate(-90deg);
			}
		}
	}
</style>