<script>
    
  import Logo from "$lib/images/Logo.png";
</script>
  <nav>
    <div class="logo">
      <!-- svelte-ignore a11y-missing-attribute -->
      <img src={Logo} />
    </div>
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
  </nav>

  <style lang="scss">
    nav {
      position: absolute;
      top: 0;
      left: 0;
      z-index: 1;
      margin: 0;
      width: 100%;
      height: 88px;
      display: block;
      flex-direction: row;
      align-items: center;
      padding: 24px 60px;
      gap: 804px;
      box-sizing: border-box;

      .logo {
        width: 206px;
        height: 32px;
        /* Inside auto layout */
        flex: none;
        order: 0;
        flex-grow: 0;
        float: left;
      }
      .content {
				/* Auto layout */
				display: flex;
				flex-direction: row;
				justify-content: center;
				align-items: center;
				padding: 0px;
				gap: 24px;

				width: 310px;
				height: 40px;

				/* Inside auto layout */
				flex: none;
				order: 1;
				flex-grow: 0;

        float: right;

				.buttons {
					/* Auto layout */
					display: flex;
					flex-direction: row;
					justify-content: center;
					align-items: center;
					padding: 0px;
					gap: 8px;

					width: 246px;
					height: 40px;

					/* Inside auto layout */
					flex: none;
					order: 0;
					flex-grow: 0;

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
						color: #FFFFFF;
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

					/* Inside auto layout */
					flex: none;
					order: 1;
					flex-grow: 0;
					border: none;
					background: transparent;
					background-image: url("../../lib/images/Burger.png");
				}
			}
    }
  </style>