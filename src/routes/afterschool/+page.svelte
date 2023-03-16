<script>
	import sports_hero from "$lib/images/Sports_logo.png";
	import logo from "$lib/images/Logo.png";
	import burger from "$lib/images/Burger.png";
	import reason_image1 from "$lib/images/reason_image1.png";
	import reason_image2 from "$lib/images/reason_image2.png";
	import point_image from "$lib/images/points_image.png";
	import learnmore from "$lib/images/learnmore.png";
	import { quintOut } from 'svelte/easing';
	import { crossfade } from 'svelte/transition';
	import { flip } from 'svelte/animate';

	const [send, receive] = crossfade({
		fallback(node, params) {
			const style = getComputedStyle(node);
			const transform = style.transform === 'none' ? '' : style.transform;

			return {
				duration: 600,
				easing: quintOut,
				css: t => `
					transform: ${transform} scale(${t});
					opacity: ${t}
				`
				
			};
		}
	});

	let todos = [
		{ id: 1, show:true, title: "asd", description: 'write some docs' },
		{ id: 2, show:false, title: "qwe", description: 'start writing JSConf talk' }
	];

	let uid = 1;

	function change() {
		console.log("asdfasdf");
		todos[0].show = todos[uid].show ? false : true;
		todos[1].show = ! todos[0].show;

	}
</script>
<svelte:head>
	<title>afterschool</title>
	<meta name="description" content="afterschool" />
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
				<h2>After School</h2>
				<span class="subtitle bodyR">Bloomingdale's After school program is a partnership with the Ombrello academy. The goal of the program is to provide enrichment activities that supplement the education experience at BIS</span>
			</div>
		</div>
		<div class="intro gradient">
			<div class="content">
				<h3 style="float:left; margin-top:0;">After School programs</h3>
				<span class="paragraph">Afterschool programs at the Galileo campus serve children of all ages and encompass a broad range of focus areas including arts, sports, and mentoring. The activities in which children and youth engage while outside of school hours are critical to their development, highlighting the need for quality afterschool programs in all communities.<br><br>

					Bloomingdale’s Afterschool program is initiated in association with the Ombrello academy that aims to provide after-school activities to further enrich and supplement the education experience at BIS for our students. We have put every effort into building a solid program, which is both fun and rewarding. Activities include sports, crafts, language, technology, and performing arts among others, and vary by term.<br><br>
					
					Activities have included: Cooking Class, Football, Basketball, Tennis, Swimming, Arts, etc.</span>
			</div>
		</div>
		<div class="points white">
			<div class="title_subtitle">
				<h2>Athletics</h2>
				<span class="subtitle bodyR">The Athletic program at BIS is committed to developing student athletes to their full potential, while also offering recreational sports for all students. Our program fosters the development of character, lifetime wellness skills, teamwork, sportsmanship, and integrity. We offer a wide range of individual and team sports for students in Kindergarten through Grade 12. </span>
			</div>
			<div class="dropdown_img">
				<div class="link">
					<div class="linkitem">
						<div class="text_arrow">
							<h5>Football</h5>
							<div class="btn_text">
								<span class="nore btn">Learn more</span>
								<div class="learnmore">
									<img src={(learnmore)} alt="">
								</div>
							</div>
						</div>
					</div>
					<div class="linkitem">
						<div class="text_arrow">
							<h5>Basketball</h5>
							<div class="btn_text">
								<span class="nore btn">Learn more</span>
								<div class="learnmore">
									<img src={(learnmore)} alt="">
								</div>
							</div>
						</div>
					</div>
					<div class="linkitem">
						<div class="text_arrow">
							<h5>Swimming</h5>
							<div class="btn_text">
								<span class="nore btn">Learn more</span>
								<div class="learnmore">
									<img src={(learnmore)} alt="">
								</div>
							</div>
						</div>
					</div>
					<div class="linkitem">
						<div class="text_arrow">
							<h5>Tennis</h5>
							<div class="btn_text">
								<span class="nore btn">Learn more</span>
								<div class="learnmore">
									<img src={(learnmore)} alt="">
								</div>
							</div>
						</div>
					</div>
					<div class="linkitem">
						<div class="text_arrow">
							<h5>Valleyball</h5>
							<div class="btn_text">
								<span class="nore btn">Learn more</span>
								<div class="learnmore">
									<img src={(learnmore)} alt="">
								</div>
							</div>
						</div>
					</div>
					<div class="linkitem">
						<div class="text_arrow">
							<h5>Track and Field</h5>
							<div class="btn_text">
								<span class="nore btn">Learn more</span>
								<div class="learnmore">
									<img src={(learnmore)} alt="">
								</div>
							</div>
						</div>
					</div>
					<div class="linkitem">
						<div class="text_arrow">
							<h5>Table Tennis</h5>
							<div class="btn_text">
								<span class="nore btn">Learn more</span>
								<div class="learnmore">
									<img src={(learnmore)} alt="">
								</div>
							</div>
						</div>
					</div>
					<div class="linkitem">
						<div class="text_arrow">
							<h5>Badminton</h5>
							<div class="btn_text">
								<span class="nore btn">Learn more</span>
								<div class="learnmore">
									<img src={(learnmore)} alt="">
								</div>
							</div>
						</div>
					</div>
					<div class="linkitem">
						<div class="text_arrow">
							<h5>Gymnastic</h5>
							<div class="btn_text">
								<span class="nore btn">Learn more</span>
								<div class="learnmore">
									<img src={(learnmore)} alt="">
								</div>
							</div>
						</div>
					</div>
				</div>
				<div class="point_image">
					<img src={(point_image)} alt="">
				</div>
			</div>
		</div>
		<div class="reasons yellow">
			<h1>1.</h1>
			<div class="reason_image1">
				<img src={(reason_image1)} alt="">
			</div>
			{#each todos.filter(t => !t.show) as todo (todo.id)}
			<div class="title_subtitle" in:receive="{{key: todo.id}}" out:send="{{key: todo.id}}" animate:flip>
				<h2>{todo.title}</h2>
				<span class="subtitle bodyR">{todo.description}</span>
			</div>
			{/each}
			<!-- svelte-ignore a11y-click-events-have-key-events -->
			<button class="scroll body2R" on:click="{() => change()}">Scroll Down</button>
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
			height: 756px;
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
					opacity: 0.6;
					position: absolute;
					right: 60px;
					width: 648px;
					float: right;
				}
			}
		}
		.points {
			width: 1440px;
			height: 1720px;
			left: 0px;
			margin-top: -80px;
			gap: 10px;
			position: relative;
			border-radius: 48px;
			z-index: -8;
			.title_subtitle {
				position: absolute;
				top: 128px;
				left: 230px;
				width: 980px;
				height: 237px;
				h2 {
					margin-top: 0;
					text-align: center;
				}
				.subtitle {
					margin: 70px;
					opacity: 0.6;
				}
			}
			.dropdown_img {
				position: absolute;
				width: 1320px;
				height: 1050px;
				left: 60px;
				top: 463px;
				.point_image {
					position: absolute;
					left: 732px;
				}
				.link {
					position: absolute;
					width: 536px;
					height: 1050px;
					padding: 0,0,48px;
					.linkitem {
						position: relative;
						gap: 32px;
						margin-top: 8%;
						top:auto;
						width: 536px;
						height: 69px;
						border-bottom: 1px solid rgba(30, 21, 21, 0.2);
						.text_arrow {
							height: 29px;
							width: 100%;
							position: absolute;
							h5 {
								margin: 0%;
								position: absolute;
							}
							.btn_text {
								position: absolute;
								height: 29px;
								width: 120px;
								left : 410px;
								.more {
									position: absolute;
									width: 86px;
									left:0%;
								}
								.learnmore {
									position: absolute;
									margin-top: -20px;
									left:86px;
								}	
							}
						}
					}
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