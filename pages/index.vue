<template>
	<div class="wrapper about-page">

		<div class="header-1">
			<div class="page-header header-filter">
				<div class="page-header-image" style="background-image: url('img/coronaton/holding-hands.jpg'); opacity: 0.45"></div>
				<div class="content-center">
					<div class="container">
						<div class="row">
							<div class="col-md-7 ml-auto text-right">
								<h1 class="title">GeoAyudas</h1>
								<h4 class="description">Gestionamos tus donaciones para la población más vulnerable, afectada por el Coronavirus COVID-19 de acuerdo a sus necesidades y ubicación</h4>
								<br />
								<div class="buttons">
									<a href="https://twitter.com" class="btn btn-icon btn-link btn-neutral btn-lg">
										<i class="fab fa-twitter"></i>
									</a>
									<a href="https://facebook.com" class="btn btn-icon btn-link btn-neutral btn-lg">
										<i class="fab fa-facebook-square"></i>
									</a>
									<a href="https://instagram.com" class="btn btn-icon btn-link btn-neutral btn-lg">
										<i class="fab fa-instagram"></i>
									</a>
								</div>
								<div class="buttons">
									<a href="./starter/#donation-button" class="btn btn-info btn-lg mr-3" target="_blank">
										Done Aquí
									</a>
									<a href="https://forms.gle/YRYiD2H88aPvi51H9" class="btn btn-primary btn-lg mr-3">
										Regístrese como beneficiario
									</a>									
								</div>								
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>


		<div class="projects-5" id="corona-solution" style="display: none">
			<div class="container">
				<div class="row">
					<div class="col-md-8 ml-auto mr-auto text-center">
						<h2 class="title">¿Qué es Coronatón?</h2>
						<h4 class="description">This is the paragraph where you can write more details about
							your projects. Keep you user engaged by providing meaningful information.</h4>
						<div class="section-space"></div>
					</div>
				</div>
				<div class="row">
					<div class="col-md-5 ml-auto">
						<card type="background" raised class="card-background-product"
							style="background-image: url('img/project8.jpg')">
							<h2 class="card-title">Social Analytics</h2>
							<p class="card-description">
								Insight to help you create, connect, and convert. Understand Your Audience's
								Interests, Influence, Interactions, and Intent. Discover emerging topics and
								influencers to reach new audiences.
							</p>
							<badge type="neutral">Analytics</badge>
						</card>
					</div>
					<div class="col-md-5 mr-auto">
						<info-section type="danger" icon="now-ui-icons ui-2_chat-round" title="Listen to Social Conversations"
							description="Gain access to the demographics, psychographics, and location of unique people who talk about your brand." />

						<info-section type="danger" icon="now-ui-icons business_chart-pie-36" title="Performance Analyze"
							description="Unify data from Facebook, Instagram, Twitter, LinkedIn, and Youtube to gain rich insights from easy-to-use reports." />

						<info-section type="danger" icon="now-ui-icons design-2_ruler-pencil" title="Social Conversions"
							description="Track actions taken on your website that originated from social, and understand the impact on your bottom line." />
					</div>
				</div>
				<hr />
				<div class="row">
					<div class="col-md-5 ml-auto mt-5">
						<info-section type="warning" icon="now-ui-icons users_single-02" title="Work With Any Team"
							description="Whether it’s for work or even the next family vacation, Trello helps your team." />

						<info-section type="warning" icon="now-ui-icons business_chart-bar-32" title="A Productivity Platform"
							description="Integrate the apps your team already uses directly into your workflow." />

						<info-section type="warning" icon="now-ui-icons arrows-1_refresh-69" title="Always In Sync"
							description="No matter where you are, Trello stays in sync across all of your devices." />

					</div>
					<div class="col-md-5 mr-auto">
						<card type="background" raised class="card-background-product"
							style="background-image: url('img/project9.jpg')">
							<h2 class="card-title">Trello lets you work.</h2>
							<p class="card-description text-white">
								Trello’s boards, lists, and cards enable you to organize and prioritize your
								projects in a fun, flexible and rewarding way.
							</p>
							<badge type="neutral">Trello</badge>
						</card>
					</div>
				</div>
			</div>
		</div>

		<div class="about-description text-center" id="donation-map">
			<div class="features-3">
				<div class="container">
					<div class="row">
						<div class="col-md-8 mr-auto ml-auto">
							<h2 class="title">Mapa de población vulnerable y coronavirus</h2>
							<h4 class="description">A través de este mapa logramos identificar la ubicación de la población 
								vulnerable en Cundinamarca y Bogotá, con el fin de gestionar las donaciones de forma eficiente.
							</h4>
						</div>
					</div>
					<div class="row">
						<div class="col-sm-12 col-md-9 ml-auto mr-auto">
							<div class="embed-container"><iframe width="500" height="400" frameborder="0" scrolling="no" marginheight="0"
									marginwidth="0" title="Testing 01"
									src="//www.arcgis.com/apps/Embed/index.html?webmap=13106e3344d64fd28254ece3b3e3885f&extent=-80.3107,0.3572,-69.5441,7.0519&zoom=true&previewImage=false&scale=true&disable_scroll=true&theme=light"></iframe>
							</div>							
						</div>
					</div>
					<div class="row">
						<col-6 class="ml-auto mr-auto">
						<a href="https://vaki.co/vaki/CoronatonColombia" target="_blank">
							<button class="btn btn-success btn-round mt-4 btn-lg" id="donation-button">
								¡Dona!
							</button>												
						</a>
						
						</col-6>
					</div>
				</div>
			</div>
		</div>

		<div class="about-team team-4">


			<div class="container">
				<div class="row">
					<div class="col-md-8 ml-auto mr-auto text-center">
						<h2 class="title">Nuestro equipo</h2>
						<h4 class="description">Somos un equipo multidisciplinario, con el único objetivo de ayudar a la población más vulnerable mediante el uso de la tecnología.</h4>
					</div>
				</div>

				<div class="row">
					<div v-for="member in team" :key="member.id" class="col-xl-6 col-lg-7 ml-auto mr-auto">
						<card type="profile" plain>
							<div slot="raw-content" class="row">
								<div class="col-md-5">
									<div class="card-image">
										<a :href="member.linkedin">
											<img class="img img-raised rounded" :src="member.picture" />
										</a>
									</div>
								</div>
								<div class="col-md-7">
									<div class="card-body">
										<h4 class="card-title">{{ member.name }}</h4>
										<h6 class="category">{{ member.position }}</h6>
										<p class="card-description">{{ member.description }}</p>
										<div class="card-footer">
											<a :href="member.linkedin" class="btn btn-icon btn-neutral btn-twitter"><i class="fab fa-linkedin"></i></a>
										</div>
									</div>
								</div>
							</div>
						</card>							
					</div>
				</div>
			</div>
		</div>

		<div class="section" style="display: none">
			<div class="about-office">
				<div class="container">
					<div class="row text-center">
						<div class="col-md-8 ml-auto mr-auto">
							<h2 class="title">Our office is our second home</h2>
							<h4 class="description">Here are some pictures from our office. You can see the place
								looks like a palace and is fully equiped with everything you need to get the job
								done.</h4>
						</div>
					</div>
					<div class="row">
						<div class="col-md-4">
							<img class="rounded img-raised" alt="Raised Image" src="img/bg27.jpg">
						</div>
						<div class="col-md-4">
							<img class="rounded img-raised" alt="Raised Image" src="img/bg24.jpg">
						</div>
						<div class="col-md-4">
							<img class="rounded img-raised" alt="Raised Image" src="img/bg28.jpg">
						</div>
						<div class="col-md-6">
							<img class="rounded img-raised" alt="Raised Image" src="img/project6.jpg">
						</div>
						<div class="col-md-6">
							<img class="rounded img-raised" alt="Raised Image" src="img/project14.jpg">
						</div>
					</div>
				</div>
			</div>
			<div class="about-contact">
				<div class="container">
					<div class="row">
						<div class="col-md-8 mr-auto ml-auto">
							<h2 class="text-center title">Want to work with us?</h2>
							<h4 class="text-center description">Divide details about your product or agency work
								into parts. Write a few lines about each one and contact us about any further
								collaboration. We will get back to you in a couple of hours.</h4>
							<form class="contact-form">
								<div class="row">
									<div class="col-md-4">
										<label>First name</label>
										<fg-input addon-left-icon="now-ui-icons users_circle-08" v-model="form.firstName"
											placeholder="First Name...">
										</fg-input>
									</div>
									<div class="col-md-4">
										<label>Your email</label>
										<fg-input addon-left-icon="now-ui-icons ui-1_email-85" v-model="form.email"
											placeholder="Email Here...">
										</fg-input>
									</div>
									<div class="col-md-4">
										<label>Speciality</label>
										<fg-input>
											<el-select class="select-default" v-model="form.speciality">
												<el-option class="select-default" value="1" label="I'm a Designer"></el-option>
												<el-option class="select-default" value="2" label="I'm a Developer"></el-option>
												<el-option class="select-default" value="3" label="I'm a Hero"></el-option>
											</el-select>
										</fg-input>
									</div>
								</div>
								<div class="row">
									<div class="col-md-4 ml-auto mr-auto text-center">
										<button class="btn btn-success btn-round mt-4 btn-lg">
											Let's talk
										</button>
									</div>
								</div>
							</form>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>
<script>
	import {
		Card,
		Button,
		Badge,
		InfoSection,
		FormGroupInput,
		Checkbox
	} from '@/components';
	import {
		Select,
		Option
	} from 'element-ui'
	import initParallax from '@/utils/initParallax'
	export default {
		name: 'about-us',
		components: {
			Card,
			InfoSection,
			Badge,
			[Button.name]: Button,
			[Checkbox.name]: Checkbox,
			[FormGroupInput.name]: FormGroupInput,
			[Select.name]: Select,
			[Option.name]: Option,
		},
		data() {
			return {
				form: {
					firstName: '',
					email: '',
					speciality: ''
				},
				team: [
					{
						name: 'Angélica Duque',
						position: 'Líder de Marketing',
						description: 'Profesional en Relaciones Internacionales y 15 años de experiencia en el área comercial, marketing e innovación.',
						picture: 'img/team/angelica.jpg',
						linkedin: 'https://www.linkedin.com/in/angelica-duque-echeverry/'
					},
					{
						name: 'Nicolás González',
						position: 'Jefe de relaciones públicas',
						description: 'Especialista en relaciones públicas con 10 años de experincia en marketing, servicio al cliente y emprendimiento',
						picture: 'img/team/nicolas-gonzalez.jpg',
						linkedin: 'https://www.linkedin.com/in/nicolas-gonzalez-delgado-89b28610a/'
					},
					{
						name: 'Nicolás García',
						position: 'Product Manager',
						description: 'Diseñador con 3 años de experiencia creando productos digitales para agencias y startups',
						picture: 'img/team/nicolas-garcia.jpg',
						linkedin: 'https://www.linkedin.com/in/nicolasgardila'
					},
					{
						name: 'Isabel Marín',
						position: 'Desarrolladora Backend',
						description: 'Ingeniera mecatrónica con experiencia en sistemas de agricultura de precisión y desarrollo backend',
						picture: 'img/team/isabel.jpg',
						linkedin: 'https://www.linkedin.com/in/maisabelmarinh/'
					},
					{
						name: 'Julián Patarroyo',
						position: 'Diseñador UX/UI',
						description: 'Diseñador UX/UI con más de 5 años de experiencia en diseño de marcas, diseño de productos digitales y marketing digital',
						picture: 'img/team/julian.jpg',
						linkedin: 'https://www.linkedin.com/in/julianpatarroyo/'
					},
					{
						name: 'Diana Hurtado',
						position: 'Especialista en GIS',
						description: 'Ingeniera Forestal con experiencia en procesos de consulta previa, sistemas de información geográfica y desarrollo web, ',
						picture: 'img/team/diana.jpg',
						linkedin: 'https://www.linkedin.com/in/dianacarolinahurtadoh/'
					},								
					{
						name: 'David Carvajal',
						position: 'Desarrollador fullstack',
						description: 'Ingeniero Electrónico y Mecánico con 10 años de experiencia y desarrollo de productos en energía, agricultura, y blockchain.',
						picture: 'img/team/david.jpg',
						linkedin: 'https://www.linkedin.com/in/dacarva'
					},
					{
						name: 'Juan Sarmiento',
						position: 'Analista financiero',
						description: 'Ingeniero industrial con énfasis en las areas de finanzas y producción. Con Experiencia en el sector petrolero y en marketing.',
						picture: 'img/team/juan.jpg',
						linkedin: 'https://www.linkedin.com/in/juansarmientoc/'
					},					
					{
						name: 'Rafael Donado',
						position: 'Gerente financiero',
						description: 'Analista de inversión con 8 años de experiencia en IFC (World Bank) en proyectos de alto impacto para el sector agrícola y farmacéutico.',
						picture: 'img/team/rafael.jpg',
						linkedin: 'https://www.linkedin.com/in/jose-rafael-donado-vallejo-2a90a1b0/'
					},										
				]
			}
		},
		mounted() {
			initParallax()
		}
	}
</script>
<style>
	.embed-container {
		position: relative;
		padding-bottom: 80%;
		height: 0;
		max-width: 100%;
	}

	.embed-container iframe,
	.embed-container object,
	.embed-container iframe {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
	}

	small {
		position: absolute;
		z-index: 40;
		bottom: 0;
		margin-bottom: -15px;
	}
</style>