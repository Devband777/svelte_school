<script>
	import Herobg from "$lib/images/layer1_back.png";
	import Videbg from "$lib/images/video.png";
	import BGgradient from "$lib/images/BGGradient.png";
	import School from "$lib/images/school.png";
	import Photo from "$lib/images/img1.png";
	import Student1 from "$lib/images/student1.png";
	import Student2 from "$lib/images/student2.png";
	import logo from "$lib/images/Logo.png";
	import arrow from "$lib/images/Arrow.png";
	import Jobcard from '../component/jobcard.svelte';
</script>

<svelte:head>
	<title>Homepage</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>
	<div class="container">
		<div class="row">
			<Jobcard/>
		</div>
	</div>
<style lang="">
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
	.events {
		box-sizing: border-box;
		position: absolute;
		
		align-items: center;
	}
	.event {
		display: flex;
		flex-direction: row;
		align-items: flex-start;
		padding: 24px;
		gap: 305px;
		isolation: isolate;
		width: 200%;
		height: 200px;
		background: #FFFFFF;
		border-radius: 24px;
	}
	.event_detail {
		display: flex;
		flex-direction: row;
		align-items: center;
		padding: 0px;
		gap: 24px;
		width: 573px;
		height: 152px;
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
		float: left;
		font-family: 'Suisse Intl';
		font-style: normal;
		font-weight: 500;
		font-size: 16px;
		line-height: 100%;
		text-align: center;
		color: #FFFFFF;
		flex: none;
		order: 0;
		flex-grow: 0;
	}
	
</style>
