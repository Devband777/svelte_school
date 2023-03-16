<script>
	import Herobg from "$lib/images/aboutus.png";
	import Videbg from "$lib/images/video.png";
	import BGgradient from "$lib/images/BGGradient.png";
	import School from "$lib/images/school.png";
	import Photo from "$lib/images/img1.png";
	import logo from "$lib/images/Logo.png"
	import Burger from "$lib/images/Burger.png"
	import Video1 from "$lib/images/Video1.png";
	import Book from "$lib/images/book1.png";
	import Paper from "$lib/images/Paper.png";
	import Board from "$lib/images/Board.png";
	import School3 from "$lib/images/school3.png"
	import School2 from "$lib/images/school2.png"
	import BGgradient1 from "$lib/images/GradientBG.png";
	import Woman from "$lib/images/IMAGE.png";
	import Playbutton from "$lib/images/playbutton.png"
	import Earth from "$lib/images/illustrations.png"
	import Notice from "$lib/images/illustrations1.png"
	import Message from "$lib/images/illustrations3.png"
	import Small from "$lib/images/illustrations4.png"
	import Bpaper from "$lib/images/illustrations5.png"
	import Man from "$lib/images/Man.png"
	import Academics from "$lib/images/academics.png"
	import Books from "$lib/images/books.png"
	import Planet from "$lib/images/planet.png"
</script>

<svelte:head>
	<title>Homepage</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>
	<div class="aboutus">
		<div class="container">
			<div class="row">
				<div class="column" style="background: url({Academics}); width:100%;height:900px">
					<div class="row">
						<div class="column1">
							<div class="row">
								<img src={logo}/>
								<div class="column"><button style="position:absolute;left:70%;top:4%;display:flex;flex-direction:row;justify-content:center;align-items:center;background:transparent;border:0;gap: 10px;"><p style="width: 85px;height: 16px;font-family: 'Suisse Intl';	font-style: normal;	font-weight: 500;font-size: 16px;line-height: 100%;color: #FFFFFF;flex: none;order: 0;flex-grow: 0;">Virtual</p></button></div>
								<div class="column"><button style="position:absolute;left:80%;top:4%;display:flex;flex-direction:row;justify-content:center;align-items:center;padding: 12px 24px;gap: 10px;width: 105px;height: 40px;background: #FFFFFF;border-radius: 100px;">Enquiry</button></div>
								<div class="column"><img src={Burger} style="position:absolute;left:90%;top:4%"/></div>
							</div>
						</div>
						<div class="column1">
							<p style="width: 600px;height: 140px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 100px;line-height: 140%;color: white;flex: none;order: 1;flex-grow: 0;position:absolute;left:4%; top:3%;">Academics</p>
							<p style="width: 400px;height: 70;font-family: 'Suisse Intl';font-style: normal;font-weight: 200;font-size: 30px;line-height: 170%;color: white;flex: none;order: 1;flex-grow: 0;position:absolute;left:4%; transform:translate(10%,30%)">To enhance learning opportunities for all children by recognising each child's unique individuality academics, social and cultural strengths and interests.</p>
						</div>
					</div>
				</div>
				<div class="column" style="margin-top:-10%;z-index;100px">
					<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 32px 72px;gap: 48px;isolation: isolate;position: absolute;width: 312px;height:360px;left: 1%;top: 40%;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 24px;">
						<img src={Earth}>
						<h1 style="text-align:center">Early years</h1>
						<p style="margin-top: -10%; text-align:center">The program is for the youngest children who grow and develop very quickly.</p>

					</div>
					<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 32px 72px;gap: 48px;isolation: isolate;position: absolute;width: 312px;height:360px;left: 46%;top: 58%;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 24px;z-index:5;">
						<img src={Books}>
						<h1 style="text-align:center">Primary years</h1>
						<p style="margin-top: -10%; text-align:center">The program is for the youngest children who grow and develop very quickly.</p>
					</div>
					<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 32px 72px;gap: 48px;isolation: isolate;position: absolute;width: 312px;height:360px;left: 23%;top: 51%;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 24px;z-index:5;">
						<img src={Book}>
						<h1 style="text-align:center">Primary years</h1>
						<p style="margin-top: -10%; text-align:center">The program is for the youngest children who grow and develop very quickly.</p>
					</div>
					<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 32px 72px;gap: 48px;isolation: isolate;position: absolute;width: 312px;height:360px;left: 10%;top: 70%;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 24px;z-index:5;">
						<img src={Small}>
						<h1 style="text-align:center">Primary years</h1>
						<p style="margin-top: -10%; text-align:center">The program is for the youngest children who grow and develop very quickly.</p>
					</div>
					<div style="position: absolute;width: 560px;height: 129px;left: 31%;top: 43%;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 36px;line-height: 120%;text-align: center;color: #254B6A;">
						<p style="text-align:center">Academics Facts</p>
					</div>
					<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 32px 72px;gap: 48px;isolation: isolate;position: absolute;width: 312px;height:360px;left: 70%;top: 63%;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 24px;z-index:5;">
						<img src={Planet}>
						<h1 style="text-align:center">Primary years</h1>
						<p style="margin-top: -10%; text-align:center">The program is for the youngest children who grow and develop very quickly.</p>
					</div>
					<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 32px 72px;gap: 48px;isolation: isolate;position: absolute;width: 312px;height:360px;left: 70%;top: 45%;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 24px;">
						<img src={Message}>
						<h1 style="text-align:center">Middle years</h1>
						<p style="margin-top: -10%; text-align:center">The program is for the youngest children who grow and develop very quickly.</p>
					</div>
					<img src={School} style="position:absolute; margin-top:39%;"/>
					<img src={BGgradient} style="border-radius:42px"/>
				</div>
				<div class="column" style="position: absolute; margin-top: -10%;">
					<div style="background:#A6D6C9;width:100%;height:auto;border-radius: 48px;">
						<div class="row">
							<div class="column1" style="margin-left:-5%;width:50%;height: 160px;">
								<p style="position: absolute;width: 1400px;height: 160px;left: -1049px;top: 72px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 160px;line-height: 100%;color: #FFFFFF;margin-top:-1%">School for creators</p>
							</div>
							<div class="column1">
								<img src={School2} style="width: 260px;height: 160px;left: 199px;position:absolute;margin-top:-80px"/> 
							</div>
							<div class="column1">
								<p style="position: absolute;width: 1400px;height: 160px;left: 507px;top: 72px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 160px;line-height: 100%;color: #FFFFFF;margin-top:-1%">School for Creators</p>
							</div>
						</div>
					</div>
				</div>
				<div class="column" style="position: absolute; margin-top: 5%;">
					<div style="background:url('{Videbg}');width:100%;height:auto;border-radius: 48px;">
						<div class="row">
							<div class="column1" style="margin-left: -1%;">
								<p style="font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 56px;line-height: 120%;color: #FFFFFF;width">
								</p>
								<p style="width: 447px;height: 140px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 20px;line-height: 140%;color: #FFFFFF;flex: none;order: 1;flex-grow: 0;"></p>
							</div>
						</div>
					</div>
				</div>
				<div class="column" style="position: absolute; margin-top: 35%;">
					<div style="background:#FFFFFF;width:100%;height:auto;border-radius: 48px;">
						<div class="row">
							<div class="column1"style="margin-left:-5%">
								<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 32px 72px;gap: 48px;isolation: isolate;position: absolute;width: 312px;height:360px;left: 1%;top: 20%;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 24px;">
									<img src={Earth}>
									<h1 style="text-align:center">Early years</h1>
									<p style="margin-top: -10%; text-align:center">The program is for the youngest children who grow and develop very quickly.</p>
			
								</div>
							</div>
							<div class="column1" style="margin-left: 12%;">
								<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 32px 72px;gap: 48px;isolation: isolate;position: absolute;width: 312px;height:360px;left: 35%;top: 20%;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 24px;">
									<img src={Earth}>
									<h1 style="text-align:center">Early years</h1>
									<p style="margin-top: -10%; text-align:center">The program is for the youngest children who grow and develop very quickly.</p>
			
								</div>
							</div>
							<div class="column1" style="margin-left: 12%;">
								<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 32px 72px;gap: 48px;isolation: isolate;position: absolute;width: 312px;height:360px;left: 71%;top: 20%;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 24px;">
									<img src={Earth}>
									<h1 style="text-align:center">Early years</h1>
									<p style="margin-top: -10%; text-align:center">The program is for the youngest children who grow and develop very quickly.</p>
								</div>
							</div>
						</div>
					</div>
				</div>
				<div class="column" style="position: absolute;margin-top:30%;">
					<div class="row">
						<div class="column1">
							<div style="width:30.5%;height: 215px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 36px;line-height: 120%;color: #1E1515;flex: none;order: 0;flex-grow: 0;position:absolute;left:2%;margin-top:40%;">
								Parents' feedback about our school. We provide an environment where we teach students how to think rather than what to think.
							</div>
						</div>
						<div class="column1">
							<div style="display: flex;flex-direction: column;align-items:justify;padding:48px;gap: 48px; flex-start;gap: 40px;position: absolute;background: #FFFFFF;border-radius: 24px;left:50%;margin-top:40%;isolation: isolate;overflow-wrap: break-word">
								<div class="row">
									<p style="width: 522px;height: 84px;font-family:'Suisse Intl';font-style: normal;font-weight: 500;font-size: 20px;line-height: 140%;color: #1E1515;flex: none;order: 0;lign-self: stretch;flex-grow: 0;text-align:justify">At Bloomingdale, Performing Arts, and well-being and life skills are taught too, which are essential for cognitive development and overall growth of the children</p>
								</div>
								<div class="row">
									<div style="display: flex;flex-direction: column;align-items: flex-start;padding: 0px;gap: 4px;width: 552px;height: 54px;flex: none;order: 1;lign-self: stretch;flex-grow: 0;margin-top:-6%">
										<p style="width: 552px;height: 28px;font-family: 'Suisse Intl';font-style: normal;font-weight: 500;font-size: 20px;line-height: 140%;color: #1E1515;
										">Mike Kaszuk</p>
										<p style="left;3%:width: 552px;height: 28px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 16px;line-height: 140%;color: #1E1515;margin-top:-4%">Mike Kaszuk</p>
									</div>
								</div>
								<div class="row">
									<div class="image-div">
										<img src={Woman} style=""/>
										<img src={Playbutton} style="position: absolute;transform:translate(-100%,10%)"/>
									</div>
								</div>
							</div>
						</div>
						<div class="column1">
							<div style="display: flex;flex-direction: column;align-items:justify;padding:48px;gap: 48px; flex-start;gap: 40px;position: absolute;background: #FFFFFF;border-radius: 24px;left:50%;isolation: isolate;overflow-wrap: break-word;margin-top:70%">
								<div class="row">
									<p style="margin:5%;width: 522px;height: 84px;font-family:'Suisse Intl';font-style: normal;font-weight: 500;font-size: 20px;line-height: 140%;color: #1E1515;flex: none;order: 0;lign-self: stretch;flex-grow: 0;text-align:justify">At Bloomingdale, Performing Arts, and well-being and life skills are taught too, which are essential for cognitive development and overall growth of the children</p>
								</div>
								<div class="row">
									<div style="display: flex;flex-direction: column;align-items: flex-start;padding: 0px;gap: 4px;width: 552px;height: 54px;flex: none;order: 1;lign-self: stretch;flex-grow: 0;margin-top:-6%">
										<p style="width: 552px;height: 28px;font-family: 'Suisse Intl';font-style: normal;font-weight: 500;font-size: 20px;line-height: 140%;color: #1E1515;
										">Mike Kaszuk</p>
										<p style="left;3%:width: 552px;height: 28px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 16px;line-height: 140%;color: #1E1515;margin-top:-4%">Mike Kaszuk</p>
									</div>
								</div>
								<div class="row">
									<div class="image-div">
										<img src={Woman} style=""/>
										<img src={Playbutton} style="position: absolute;transform:translate(-100%,10%)"/>
									</div>
								</div>
							</div>
						</div>
						<div style="top:20%">
							<div class="column1">
								<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 30px;gap: 48px;width: 312px;height: 312px;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 20px;flex: none;order: 0;flex-grow: 0;position:absolute;top:75%;left:1%;">
									<div class="row" style="margin-top: -30%;">
										<p style="width: 151px;height: 80px;font-family: 'Suisse Intl';font-style: normal;font-weight: 500;font-size: 80px;line-height: 100%;text-align: center;letter-spacing: -0.02em;color: #DE8A2E;flex: none;order: 0;flex-grow: 0;">1/40</p>
									</div>
									<div class="row" style="margin-top: -40%;">
										<p style="width: 248px;height: 88px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 16px;line-height: 140%;text-align: center;color: rgba(15, 17, 33, 0.6);flex: none;order: 1;flex-grow: 0;">Schools in teh U.S. with the International Baccalaureate PYP-MYP-DP currciculum from grade PK3 through 12
										</p>
									</div>
								</div>
							</div>
							<div class="column1">
								<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 30px;gap: 48px;width: 312px;height: 312px;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 20px;flex: none;order: 0;flex-grow: 0;position:absolute;top:75%;left:25%;">
									<div class="row" style="margin-top: -30%;">
										<p style="width: 151px;height: 80px;font-family: 'Suisse Intl';font-style: normal;font-weight: 500;font-size: 80px;line-height: 100%;text-align: center;letter-spacing: -0.02em;color: #8E4B98;flex: none;order: 0;flex-grow: 0;">100%</p>
									</div>
									<div class="row" style="margin-top: -40%;">
										<p style="width: 248px;height: 88px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 16px;line-height: 140%;text-align: center;color: rgba(15, 17, 33, 0.6);flex: none;order: 1;flex-grow: 0;">Schools in teh U.S. with the International Baccalaureate PYP-MYP-DP currciculum from grade PK3 through 12
										</p>
									</div>
								</div>
							</div>
							<div class="column1">
								<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 30px;gap: 48px;width: 312px;height: 312px;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 20px;flex: none;order: 0;flex-grow: 0;position:absolute;top:75%;left:49%;">
									<div class="row" style="margin-top: -30%;">
										<p style="width: 151px;height: 80px;font-family: 'Suisse Intl';font-style: normal;font-weight: 500;font-size: 80px;line-height: 100%;text-align: center;letter-spacing: -0.02em;color: #CEDA42;flex: none;order: 0;flex-grow: 0;">12</p>
									</div>
									<div class="row" style="margin-top: -40%;">
										<p style="width: 248px;height: 88px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 16px;line-height: 140%;text-align: center;color: rgba(15, 17, 33, 0.6);flex: none;order: 1;flex-grow: 0;">Schools in teh U.S. with the International Baccalaureate PYP-MYP-DP currciculum from grade PK3 through 12
										</p>
									</div>
								</div>
							</div>
							<div class="column1">
								<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 30px;gap: 48px;width: 312px;height: 312px;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 20px;flex: none;order: 0;flex-grow: 0;position:absolute;top:75%;left:73%;">
									<div class="row" style="margin-top: -30%;">
										<p style="width: 151px;height: 80px;font-family: 'Suisse Intl';font-style: normal;font-weight: 500;font-size: 80px;line-height: 100%;text-align: center;letter-spacing: -0.02em;color: #64A8DF;flex: none;order: 0;flex-grow: 0;">48%</p>
									</div>
									<div class="row" style="margin-top: -40%;">
										<p style="width: 248px;height: 88px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 16px;line-height: 140%;text-align: center;color: rgba(15, 17, 33, 0.6);flex: none;order: 1;flex-grow: 0;">Schools in teh U.S. with the International Baccalaureate PYP-MYP-DP currciculum from grade PK3 through 12
										</p>
									</div>
								</div>
							</div>
						</div>
					</div>
					<img src={BGgradient1} style="border-radius: 20px;"/>
				</div>
				<div class="column" style="position: absolute; margin-top: 170%;">
					<div style="background: #EFDB34;width:100%;height:auto;border-radius: 48px;">
						<div class="row">
							<div class="column1"style="">
								<img src={Photo} width=400px height=500px style="left: -10%;"/>	
							</div>
							<div class="column1" style="margin-left: 20%;margin-top:-2%">
								<p style="font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 56px;line-height: 120%;color: #254B6A;width:400px;height:140px">Our School values
								</p>
								<p style="width: 447px;height: 140px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 20px;line-height: 140%;color: #254B6A;flex: none;order: 1;flex-grow: 0;">We provide an environment where we teach students how to think rather than what to think. We aim to provide memorable experiences that foster a real love of learning and personal development</p>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
<style lang="scss">
	.aboutus{
		.image-div{
			position: absolute;
			right: 0px;
			transform: translate(-20%,-15%);
		}
		.logo{
			position:absolute;
			left:5%;
			top:4%;
		}
			* {
			box-sizing: border-box;
		}
		.schoolL{
			position: absolute;
			width: 1400px;
			height: 160px;
			left: -390px;
			top: 20%;
			
			/* Desktop/Running line Desktop | 160 */

			font-family: 'Suisse Intl';
			font-style: normal;
			font-weight: 400;
			font-size: 160px;
			line-height: 100%;
			/* identical to box height, or 160px */


			/* Basic & Secondary/White */

			color: #FFFFFF;
		}
		.schoolR{
			position: absolute;
			width: 1400px;
			height: 160px;
			left: 1000px;
			top: 20%;

			/* Desktop/Running line Desktop | 160 */

			font-family: 'Suisse Intl';
			font-style: normal;
			font-weight: 400;
			font-size: 160px;
			line-height: 100%;
			/* identical to box height, or 160px */


			/* Basic & Secondary/White */

			color: #FFFFFF;
		}
		.schoolimg{
			position: absolute;
			width: 536px;
			height: 600px;
			left: 596px;
			top: 128px;
			border-radius: 24px;
			transform: matrix(-1, 0, 0, 1, 0, 0);
		}
		.container {
			position: absolute;
		}
		.row:after {
			content: "";
			display: table;
			clear: both;
		}
		.column1{
			float: left;
			width:1%;
			padding: 10%;
		}
		.column {
			float: down;
			width: 100%;
		}
	}
</style>
