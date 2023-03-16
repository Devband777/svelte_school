<script>
	import Herobg from "$lib/images/layer1_back.png";
	import Videbg from "$lib/images/video.png";
	import BGgradient from "$lib/images/BGGradient.png";
	import School from "$lib/images/school.png";
	import Photo from "$lib/images/img1.png";
	import Student1 from "$lib/images/student1.png";
	import Student2 from "$lib/images/student2.png";
	import logo from "$lib/images/Logo.png"
	import Burger from "$lib/images/Burger.png"
	import Video1 from "$lib/images/Video1.png";
	import Book from "$lib/images/book1.png";
	import Paper from "$lib/images/Paper.png";
	import Board from "$lib/images/Board.png";
	import School2 from "$lib/images/school2.png"
	import BGgradient1 from "$lib/images/GradientBG.png";
	import Woman from "$lib/images/IMAGE.png";
	import Playbutton from "$lib/images/playbutton.png"
</script>

<svelte:head>
	<title>Homepage</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>
	<div class="homepage">
		<div class="container">
			<div class="row">
				<div class="column" style="background: url({Herobg}); width:100%;height:900px">
					<div class="row">
						<div class="column1">
							<div class="row">
								<div class="column"><img src={logo}/></div>
								<div class="column"><button style="position:absolute;left:70%;top:4%;display:flex;flex-direction:row;justify-content:center;align-items:center;background:transparent;border:0;gap: 10px;"><p style="width: 85px;height: 16px;font-family: 'Suisse Intl';	font-style: normal;	font-weight: 500;font-size: 16px;line-height: 100%;color: #FFFFFF;flex: none;order: 0;flex-grow: 0;">Virtual</p></button></div>
								<div class="column"><button style="position:absolute;left:80%;top:4%;display:flex;flex-direction:row;justify-content:center;align-items:center;padding: 12px 24px;gap: 10px;width: 105px;height: 40px;background: #FFFFFF;border-radius: 100px;">Enquiry</button></div>
								<div class="column"><img src={Burger} style="position:absolute;left:90%;top:4%"/></div>
							</div>
						</div>
						<div class="column1">
							<p style="width: 600px;height: 140px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 100px;line-height: 140%;color: white;flex: none;order: 1;flex-grow: 0;position:absolute;left:4%; top:8%;">The #1 <br/><img src={Student1}/><img src={Student2} style="margin-left: -2%;"/>School for performers</p>
						</div>
					</div>
				</div>
				<div class="coloumn">
					<div style="background:#A6D6C9;width:100%;height:auto;border-radius: 48px;margin-top:-9%;">
						<div class="row">
							<div class="column1">
								<p class="schoolL">or creators</p>
							</div>
							<div class="column1">
								<img class="video_img" src={Video1} style="transform:translate(20%,-50%)"/> 
							</div>
							<div class="column1">
								<p class="schoolR">School</p>
							</div>
						</div>
					</div>
				</div>
				<div class="column">
						<img src={Videbg} style="margin-top:-5%"/>
				</div>
				<div class="column" style="margin-top:-5%">
					<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 32px 72px;gap: 48px;isolation: isolate;position: absolute;width: 312px;height:360px;left: 10%;top: 64%;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 24px;">
						<img src={Book}>
						<h1 style="text-align:center">Early years</h1>
						<p style="margin-top: -10%; text-align:center">The program is for the youngest children who grow and develop very quickly.</p>

					</div>
					<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 32px 72px;gap: 48px;isolation: isolate;position: absolute;width: 312px;height:360px;left: 40%;top: 80%;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 24px;z-index:5;">
						<img src={Paper}>
						<h1 style="text-align:center">Primary years</h1>
						<p style="margin-top: -10%; text-align:center">The program is for the youngest children who grow and develop very quickly.</p>
					</div>
					<div style="position: absolute;width: 560px;height: 129px;left: 31%;top: 69%;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 36px;line-height: 120%;text-align: center;color: #254B6A;">
						<p style="text-align:center">The program is for the youngest children who grow and develop very quickly.</p>
					</div>
					<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 32px 72px;gap: 48px;isolation: isolate;position: absolute;width: 312px;height:360px;left: 70%;top: 70%;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 24px;">
						<img src={Board}>
						<h1 style="text-align:center">Middle years</h1>
						<p style="margin-top: -10%; text-align:center">The program is for the youngest children who grow and develop very quickly.</p>
					</div>
					<img src={School} style="position:absolute; margin-top:39%;"/>
					<img src={BGgradient} style="border-radius:42px"/>
				</div>
				<div class="column" style="position: absolute; margin-top: -10%;">
					<div style="background:#EFDB34;width:100%;height:auto;border-radius: 48px;">
						<div class="row">
							<div class="column1">
								<p style="font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 160px;line-height: 0.1%; color: #254B6A;">1.</p>
							</div>
							<div class="column1"style="margin-left:-10%">
								<img src={Photo} width=auto height=auto style="left: 10%;top: 10%;"/>	
							</div>
							<div class="column1" style="margin-left: 20%;">
								<p style="font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 56px;line-height: 120%;color: #254B6A;">
								Respons to join Bloomingdale.</p>
								<p style="width: 447px;height: 140px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 20px;line-height: 140%;color: #254B6A;flex: none;order: 1;flex-grow: 0;">We provide an environment where we teach students how to think rather than what to think. We aim to provide memorable experiences that foster a real love of learning and personal development</p>
							</div>
						</div>
					</div>
				</div>
				<div class="column">
					<div style="position: absolute;width:100%;height: 50%;left: 0px;top: 3840px;background: #A6D6C9;border-radius: 40px;margin-top:-1%">
						<div class="row" style="margin-top:-5%">
							<div class="column1" style="margin-left:-5%;width:50%;height: 160px;">
								<p style="position: absolute;width: 1400px;height: 160px;left: -1049px;top: 72px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 160px;line-height: 100%;color: #FFFFFF;margin-top:-1%">School for creators</p>
							</div>
							<div class="column1">
								<img src={School2} style="width: 260px;height: 160px;left: 199px;position:absolute"/> 
							</div>
							<div class="column1">
								<p style="position: absolute;width: 1400px;height: 160px;left: 507px;top: 72px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 160px;line-height: 100%;color: #FFFFFF;margin-top:-1%">School for Creators</p>
							</div>
						</div>
					</div>
				</div>
				<div class="column" style="position: absolute;margin-top:19%;">
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
			</div>
		</div>
	</div>
<style lang="scss">
	.homepage{
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
		.video_img{
			width: 260px;
			height: 160px;
			left: 804px;
			top: 72px;
		}
		.container {
			position: absolute;
		}
		.row:after {
			content: "";
			display: table;
			clear: both;
		}
		h1 {
			width: 100%;
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
		.hero-bgimage{
			position: absolute;
			width: 80%;
			height:100%;
		}
		.video-bgimage{
			position:absolute;
			width: 80%;
			height:100%;
		}
		.image-div{
			position: absolute;
			right: 0px;
			transform: translate(-20%,-15%);
		}
	}
</style>
