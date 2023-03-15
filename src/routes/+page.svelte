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
	import arrow from "$lib/images/Arrow.png";
</script>

<svelte:head>
	<title>Homepage</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>
	<div class="container">
		<div class="row">
			<div class="column">
				<div class="row">
					<div class="column1">
						<div class="row">
							<div class="column"><img src={logo} style="position:absolute;left:5%;top:4%"/></div>
							<div class="column"><button style="position:absolute;left:70%;top:4%;display:flex;flex-direction:row;justify-content:center;align-items:center;padding:12px 24px;gap: 10px;"><p style="width: 85px;height: 16px;font-family: 'Suisse Intl';	font-style: normal;	font-weight: 500;font-size: 16px;line-height: 100%;color: #FFFFFF;flex: none;order: 0;flex-grow: 0;">Virtual</p></button></div>
<<<<<<< HEAD
							<div class="column"><button style="position:absolute;left:80%;top:4%;display:flex;flex-direction:row;justify-content:center;align-items:center;padding: 12px 24px;gap: 10px;width: 105px;height: 40px;background: #FFFFFF;border-radius: 100px;">Enquiry</button></div>
							<div class="column"><img src={Burger} style="position:absolute;left:90%;top:4%"/></div>
=======
							<div class="column"><button style="position:absolute;left:80%;top:4%;display:flex;flex-direction:row;justify-content:center;align-items:center;padding: 12px 24px;gap: 10px;width: 105px;height: 40px;background: #FFFFFF;border-radius: 100px;font-style:white;">Enquiry</button></div>
>>>>>>> 1b09527 (rat)
						</div>
					</div>
					<div class="column1">
						<p style="width: 600px;height: 140px;font-family: 'Suisse Intl';font-style: normal;font-weight: 400;font-size: 100px;line-height: 140%;color: white;flex: none;order: 1;flex-grow: 0;position:absolute;left:4%; top:8%;">The #1 <br/><img src={Student1}/><img src={Student2} style="margin-left: -2%;"/>School for performers</p>
					</div>
					<div class="column">
						<img src={Herobg}/>
					</div>
				</div>
			</div>
			<div class="coloumn">
				<div style="background:#A6D6C9;width:100%;height:auto;border-radius: 48px;margin-top:-10%;transform-y:10px">
					<div class="row">
						<div class="column1" style="margin-left:-5%;width:50%;height: 160px;left: -644px;top: 72px;">
							<p style="font-family: 'Suisse Intl';font-style: normal;font-weight: 40;font-size: 100px;line-height: 100%;color: #FFFFFF;">or creators</p>
						</div>
						<div class="column1">
							<img src={Video1} style="top:400px;"/> 
						</div>
						<div class="column1">
							<p style="font-family: 'Suisse Intl';font-style: normal;font-weight: 40;font-size: 100px;line-height: 100%;color: #FFFFFF;">School</p>
						</div>
					</div>
				</div>
			</div>
			<div class="column">
					<img src={Videbg} style="margin-top:-30%"/>
			</div>
			<div class="column" style="margin-top:-5%">
				<div>
					<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 32px 72px;gap: 48px;isolation: isolate;position: absolute;width: 312px;height:360px;left: 10%;top: 64%;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 24px;">
						<img src={Book}>
						<h1 style="text-align:center">Early years</h1>
						<p style="margin-top: -10%; text-align:center">The program is for the youngest children who grow and develop very quickly.</p>
					</div>
					<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 32px 72px;gap: 48px;isolation: isolate;position: absolute;width: 312px;height:360px;left: 40%;top: 80%;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 24px;z-index:5;">
						<img src={Book}>
						<h1 style="text-align:center">Early years</h1>
						<p style="margin-top: -10%; text-align:center">The program is for the youngest children who grow and develop very quickly.</p>
					</div>
					<div style="display: flex;flex-direction: column;align-items: center;padding: 48px 32px 72px;gap: 48px;isolation: isolate;position: absolute;width: 312px;height:360px;left: 70%;top: 70%;background: #FFFFFF;box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);border-radius: 24px;">
						<img src={Book}>
						<h1 style="text-align:center">Early years</h1>
						<p style="margin-top: -10%; text-align:center">The program is for the youngest children who grow and develop very quickly.</p>
					</div>
					<img src={School} style="position:absolute; margin-top:39%;"/>
					<img src={BGgradient} style="border-radius:42px"/>
				</div>
			</div>
			<div class="column" style="position: absolute; margin-top: -10%;">
				<div style="background:#EFDB34;width:400%;height:auto;border-radius: 48px;">
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
			<div class="column" style="position: absolute; margin-top: -10%;">
				<div style="background:#A6D6C9; width:400%; height:auto;border-radius: 48px;z-index:10;">
					<div style="display: flex;flex-direction: column;align-items: center;padding: 0px;gap: 64px;left: 172px;top: 128px;">
						<h2>Upcoming Events</h2>
						<div class="event_btn">
							<span>See all events<img src={arrow} width=28px height=28px style="flex: none;order: 1;flex-grow: 0;top:-3px;"/></span>
							
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
<style lang="sass">
	.container {
		box-sizing: border-box;
		position: absolute;
		left:9%;
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
		width: 25%;
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
	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
	h2 {
		font-family: 'Suisse Intl';
		font-style: normal;
		font-weight: 400;
		font-size: 56px;
		line-height: 120%;
		color: #254B6A;
	}
	.event_btn {
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		padding: 10px 10px 10px 24px;
		gap: 8px;
		background: #DE8A2E;
		border-radius: 24px;
		flex: none;
		order: 1;
		flex-grow: 0;	
	}
	span {
		color: #FFFFFF;
		font-family: 'Suisse Intl';
		font-style: normal;
		font-weight: 500;
		font-size: 16px;
	}
</style>
