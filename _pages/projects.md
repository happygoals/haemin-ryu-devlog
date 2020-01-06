---
layout: post
title: "Projects"
permalink: /projects/
---
<style>
	/* Tiles */
	h2, h3, h4, h5, h6 {
		font-weight: 900;
		line-height: 1.5;
		margin: 0 0 2em 0;
		text-transform: uppercase;
		letter-spacing: 0.35em;
	}

		h2 a, h3 a, h4 a, h5 a, h6 a {
			color: inherit;
		}

	h2 {
		font-size: 1.1em;
	}
	
	.tiles {
		display: -moz-flex;
		display: -webkit-flex;
		display: -ms-flex;
		display: flex;
		-moz-flex-wrap: wrap;
		-webkit-flex-wrap: wrap;
		-ms-flex-wrap: wrap;
		flex-wrap: wrap;
		postiion: relative;
		margin: -2.5em 0 0 -2.5em;
	}

		.tiles article {
			-moz-transition: -moz-transform 0.5s ease, opacity 0.5s ease;
			-webkit-transition: -webkit-transform 0.5s ease, opacity 0.5s ease;
			-ms-transition: -ms-transform 0.5s ease, opacity 0.5s ease;
			transition: transform 0.5s ease, opacity 0.5s ease;
			position: relative;
			width: calc(33.33333% - 2.5em);
			margin: 2.5em 0 0 2.5em;
		}

			.tiles article > .image {
				-moz-transition: -moz-transform 0.5s ease;
				-webkit-transition: -webkit-transform 0.5s ease;
				-ms-transition: -ms-transform 0.5s ease;
				transition: transform 0.5s ease;
				position: relative;
				display: block;
				width: 100%;
				border-radius: 4px;
				overflow: hidden;
			}

				.tiles article > .image img {
					display: block;
					width: 100%;
				}

				.tiles article > .image:before {
					pointer-events: none;
					-moz-transition: background-color 0.5s ease, opacity 0.5s ease;
					-webkit-transition: background-color 0.5s ease, opacity 0.5s ease;
					-ms-transition: background-color 0.5s ease, opacity 0.5s ease;
					transition: background-color 0.5s ease, opacity 0.5s ease;
					content: '';
					display: block;
					position: absolute;
					top: 0;
					left: 0;
					width: 100%;
					height: 100%;
					opacity: 1.0;
					z-index: 1;
					opacity: 0.8;
				}

				.tiles article > .image:after {
					pointer-events: none;
					-moz-transition: opacity 0.5s ease;
					-webkit-transition: opacity 0.5s ease;
					-ms-transition: opacity 0.5s ease;
					transition: opacity 0.5s ease;
					content: '';
					display: block;
					position: absolute;
					top: 0;
					left: 0;
					width: 100%;
					height: 100%;
					background-image: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='100' height='100' viewBox='0 0 100 100' preserveAspectRatio='none'%3E%3Cstyle%3Eline %7B stroke-width: 0.25px%3B stroke: %23ffffff%3B %7D%3C/style%3E%3Cline x1='0' y1='0' x2='100' y2='100' /%3E%3Cline x1='100' y1='0' x2='0' y2='100' /%3E%3C/svg%3E");
					background-position: center;
					background-repeat: no-repeat;
					background-size: 100% 100%;
					opacity: 0.25;
					z-index: 2;
				}

			.tiles article > a {
				display: -moz-flex;
				display: -webkit-flex;
				display: -ms-flex;
				display: flex;
				-moz-flex-direction: column;
				-webkit-flex-direction: column;
				-ms-flex-direction: column;
				flex-direction: column;
				-moz-align-items: center;
				-webkit-align-items: center;
				-ms-align-items: center;
				align-items: center;
				-moz-justify-content: center;
				-webkit-justify-content: center;
				-ms-justify-content: center;
				justify-content: center;
				-moz-transition: background-color 0.5s ease, -moz-transform 0.5s ease;
				-webkit-transition: background-color 0.5s ease, -webkit-transform 0.5s ease;
				-ms-transition: background-color 0.5s ease, -ms-transform 0.5s ease;
				transition: background-color 0.5s ease, transform 0.5s ease;
				position: absolute;
				top: 0;
				left: 0;
				width: 100%;
				height: 100%;
				padding: 1em;
				border-radius: 4px;
				border-bottom: 0;
				color: #ffffff;
				text-align: center;
				text-decoration: none;
				z-index: 3;
			}

				.tiles article > a > :last-child {
					margin: 0;
				}

				.tiles article > a:hover {
					color: #ffffff !important;
				}

				.tiles article > a h2 {
					margin: 0;
				}

				.tiles article > a .content {
					-moz-transition: max-height 0.5s ease, opacity 0.5s ease;
					-webkit-transition: max-height 0.5s ease, opacity 0.5s ease;
					-ms-transition: max-height 0.5s ease, opacity 0.5s ease;
					transition: max-height 0.5s ease, opacity 0.5s ease;
					width: 100%;
					max-height: 0;
					line-height: 1.5;
					margin-top: 0.35em;
					opacity: 0;
				}

					.tiles article > a .content > :last-child {
						margin-bottom: 0;
					}

			.tiles article.style1 > .image:before {
				background-color: #f2849e;
			}

			.tiles article.style2 > .image:before {
				background-color: #7ecaf6;
			}

			.tiles article.style3 > .image:before {
				background-color: #7bd0c1;
			}

			.tiles article.style4 > .image:before {
				background-color: #c75b9b;
			}

			.tiles article.style5 > .image:before {
				background-color: #ae85ca;
			}

			.tiles article.style6 > .image:before {
				background-color: #8499e7;
			}

			body:not(.is-touch) .tiles article:hover > .image {
				-moz-transform: scale(1.1);
				-webkit-transform: scale(1.1);
				-ms-transform: scale(1.1);
				transform: scale(1.1);
			}

				body:not(.is-touch) .tiles article:hover > .image:before {
					background-color: #333333;
					opacity: 0.35;
				}

				body:not(.is-touch) .tiles article:hover > .image:after {
					opacity: 0;
				}

			body:not(.is-touch) .tiles article:hover .content {
				max-height: 15em;
				opacity: 1;
			}

		* + .tiles {
			margin-top: 2em;
		}

		body.is-preload .tiles article {
			-moz-transform: scale(0.9);
			-webkit-transform: scale(0.9);
			-ms-transform: scale(0.9);
			transform: scale(0.9);
			opacity: 0;
		}

		body.is-touch .tiles article .content {
			max-height: 15em;
			opacity: 1;
		}

		@media screen and (max-width: 1280px) {

			.tiles {
				margin: -1.25em 0 0 -1.25em;
			}

				.tiles article {
					width: calc(33.33333% - 1.25em);
					margin: 1.25em 0 0 1.25em;
				}

		}

		@media screen and (max-width: 980px) {

			.tiles {
				margin: -2.5em 0 0 -2.5em;
			}

				.tiles article {
					width: calc(50% - 2.5em);
					margin: 2.5em 0 0 2.5em;
				}

		}

		@media screen and (max-width: 736px) {

			.tiles {
				margin: -1.25em 0 0 -1.25em;
			}

				.tiles article {
					width: calc(50% - 1.25em);
					margin: 1.25em 0 0 1.25em;
				}

					.tiles article:hover > .image {
						-moz-transform: scale(1.0);
						-webkit-transform: scale(1.0);
						-ms-transform: scale(1.0);
						transform: scale(1.0);
					}

		}

		@media screen and (max-width: 480px) {

			.tiles {
				margin: 0;
			}

				.tiles article {
					width: 100%;
					margin: 1.25em 0 0 0;
				}

		}
</style> 


[Gmail](mailto://developer.haemin.ryu@gmail.com)
[Phone](tel:260-255-2983)
[GitHub](https://github.com/happygoals)
[Portfolio](https://happygoals.github.io/)


<section class="tiles">
		<article class="style1">
			<span class="image">
				<img src="../assets/images/pic01.jpg" alt="" style="width:250px;height:250px;"/>
			</span>
			<a href="https://github.com/mfwlr/DigitalHarvestTutorial">
				<h2>Digital Harvest</h2>
				<div class="content">
					<p>I have developed a web app to meet the goal of helping food growers through online market. </p>
				</div>
			</a>
		</article>
		<article class="style2">
			<span class="image">
				<img src="../assets/images/pic02.jpg" alt="" style="width:250px;height:250px;"/>
			</span>
			<a href="https://github.com/happygoals/Team7_PFW_Capstone">
				<h2>Indoor Navigation : Improved Accessibility for People with Disabilities </h2>
				<div class="content">
					<p>This project include web development utilizing data and business analytics, targeted advertisements that will promote Parkview technologies, and improved mobile application navigation to assisted disabled patients.  </p>
				</div>
			</a>
		</article>
		<article class="style3">
			<span class="image">
				<img src="../assets/images/pic03.jpg" alt="" style="width:250px;height:250px;"/>
			</span>
			<a href="http://erc.pfw.edu/">
				<h2>Environment Resource Center</h2>
				<div class="content">
					<p> Using Wordpress, I recreated the the Environmental Resource Center websites related in the department of the biology for Purdue rebranding, herpetofauna Education and Research Program website.</p>
				</div>
			</a>
		</article>
		<article class="style4">
			<span class="image">
				<img src="../assets/images/pic04.jpg" alt="" style="width:250px;height:250px;"/>
			</span>
			<a href="http://github.com/happygoals/web_app_dev_fall2018">
				<h2>Snackfacts</h2>
				<div class="content">
					<p>Snackfacts is a vending machine marketing analytics tool. A user can input data into survey, which are the saved into our database.  The data we collect is then presented in a comprehensive analysis screen. Users can create account to save data they enter, and then the administrators can have special admin accounts. </p>
				</div>
			</a>
		</article>
		<article class="style5">
			<span class="image">
				<img src="../assets/images/pic05.jpg" alt="" style="width:250px;height:250px;"/>
			</span>
			<a href="generic.html">
				<h2>Professor's Personal Website</h2>
				<div class="content">
					<p>I developed several professors’ personal websites.</p>
				</div>
			</a>
		</article>
		<article class="style6">
			<span class="image">
				<img src="../assets/images/pic06.jpg" alt="" style="width:250px;height:250px;"/>
			</span>
			<a href="https://devpost.com/software/letmeoff-fhyj4w#">
				<h2>Let Me Off – Android(Java) </h2>
				<p>DemonHacks 2019</p>
				<div class="content">
					<p>This mobile app is for the people(Sleepyheads, forgetful heads, travelers) who miss getting off the bus when they arrive at the right bus stop.</p>
				</div>
			</a>
		</article>
		<article class="style2">
			<span class="image">
				<img src="../assets/images/pic07.jpg" alt="" style="width:250px;height:250px;"/>
			</span>
			<a href="https://www.youtube.com/watch?v=DBUaVWYqFHM&feature=youtu.be">
				<h2>Cat Back Home – Unity(C#) </h2>
				<div class="content">
					<p>This is my first game development based on the real story of a cat living in a student housing that goes out to find her real home.</p>
				</div>
			</a>
		</article>
		<article class="style3">
			<span class="image">
				<img src="../assets/images/pic08.jpg" alt="" style="width:250px;height:250px;"/>
			</span>
			<a href="https://www.youtube.com/watch?v=RtuqlmzrMhc&feature=youtu.be">
				<h2>Run On the Bass– OpenGL(C) </h2>
				<div class="content">
					<p>This is a running game that the finger runs on the bass guitar.</p>
				</div>
			</a>
		</article>
		<article class="style1">
			<span class="image">
				<img src="../assets/images/pic09.jpg" alt="" style="width:250px;height:250px;"/>
			</span>
			<a href="#">
				<h2>Coming Soon..</h2>
				<div class="content">
					<p></p>
				</div>
			</a>
		</article>
		<br>
		<br>
</section>


