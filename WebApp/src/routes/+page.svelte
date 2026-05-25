<script>
	import { goto } from '$app/navigation';
	import { onMount } from 'svelte';

	let ScreenWidth = 1080;

	onMount(() => {});
</script>

<div class="MainContainer">
	<section class="titleSection">
		<h1 id="Maintitle">Gremio Estudantil <br />Arnaldo Cardoso Rocha</h1>
	</section>
	<section class="about">
		<div class="TextContainer">
			<h1 class="SectionTitle">O que somos nos</h1>
			<p class="MinorText">
				O Grêmio Estudantil Arnaldo Cardoso Rocha é a entidade representativa dos estudantes da
				Educação Profissional Técnica de Nível Médio do CEFET-MG, com sede no campus Nova Suíça em
				Belo Horizonte. Seu papel principal é defender os interesses dos alunos, promover
				protagonismo estudantil, participar ativamente da vida acadêmica e contribuir para um
				ambiente educacional mais inclusivo, participativo e acolhedor. A entidade organiza
				atividades culturais, sociais e de acolhimento e busca fortalecer a participação dos
				estudantes nas decisões e na vida do campus, sempre incentivando o uso coletivo da sede e a
				colaboração entre pares.
			</p>
		</div>
	</section>
	<section class="pautas">
		<h1 class="SectionTitle PautasTitle">Nossas Pautas</h1>
		{#if ScreenWidth > 768}
			<div class="DecBefore"></div>
			<div class="Pautas">
				<div class="pauta">
					<h1 class="pautaTitle">Recuperaçao paralela</h1>
					<p class="MinorText">
						Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris vitae lorem ut nunc
						pretium fermentum sed sit amet ipsum. Morbi ultricies iaculis turpis id convallis.
						Suspendisse pretium mattis urna, ac porttitor enim suscipit quis. Mauris nec enim nec
						est commodo bibendum quis id libero. Praesent cursus sit amet lectus sit amet tristique.
						Cras nec auctor ante. Aliquam a dolor id nunc ornare venenatis. Phasellus condimentum
						sapien eget ligula semper, eu pulvinar nunc dignissim. Cras semper ante nec fermentum
						bibendum. Aenean.
					</p>
				</div>
				<div class="pauta">
					<h1 class="pautaTitle">Recuperaçao paralela</h1>
					<p class="MinorText">
						Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris vitae lorem ut nunc
						pretium fermentum sed sit amet ipsum. Morbi ultricies iaculis turpis id convallis.
						Suspendisse pretium mattis urna, ac porttitor enim suscipit quis. Mauris nec enim nec
						est commodo bibendum quis id libero. Praesent cursus sit amet lectus sit amet tristique.
						Cras nec auctor ante. Aliquam a dolor id nunc ornare venenatis. Phasellus condimentum
						sapien eget ligula semper, eu pulvinar nunc dignissim. Cras semper ante nec fermentum
						bibendum. Aenean.
					</p>
				</div>
				<div class="pauta">
					<h1 class="pautaTitle">Recuperaçao paralela</h1>
					<p class="MinorText">
						Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris vitae lorem ut nunc
						pretium fermentum sed sit amet ipsum. Morbi ultricies iaculis turpis id convallis.
						Suspendisse pretium mattis urna, ac porttitor enim suscipit quis. Mauris nec enim nec
						est commodo bibendum quis id libero. Praesent cursus sit amet lectus sit amet tristique.
						Cras nec auctor ante. Aliquam a dolor id nunc ornare venenatis. Phasellus condimentum
						sapien eget ligula semper, eu pulvinar nunc dignissim. Cras semper ante nec fermentum
						bibendum. Aenean.
					</p>
				</div>
			</div>
			<div class="DecAfter"></div>
		{/if}
	</section>
	<section class="participate">
		<div class="TextContainer">
			<h1 class="SectionTitle">Como participar</h1>
			<p class="MinorText">
				Todos os alunos da Educação Profissional Técnica de Nível Médio do CEFET-MG podem participar
				do Grêmio Estudantil Arnaldo Cardoso Rocha. Isso mediante a subordinaçao ao estatudo
				definido pelas assembleias e plenarias realizadas anteriormente
			</p>
		</div>
	</section>
	<div class="Ender"></div>
</div>

<style>
	section {
		width: 100dvw;
		height: fit-content;
		max-height: 90vh;
		margin-bottom: 20dvh;
	}
	.titleSection {
		width: 100dvw;
		background: url('./images/Tarifa0.png');
		height: 50dvh;
		display: flex;
		align-items: center;
		justify-content: center;
		background-repeat: no-repeat;
		background-size: cover;
		background-position-y: center;
		color: var(--Deep-Blue-Accent);
		margin-bottom: 10dvh !important;
	}
	#Maintitle {
		opacity: 100% !important;
		text-align: center;
		font-size: 5vw;
	}
	.Pautas {
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
	}
	.TextContainer {
		width: 90%;
		margin: 0 auto;
	}
	.SectionTitle {
		color: var(--Red-Accent);
		font-size: 4rem;
		font-family: 'Lora', serif;
	}
	.MinorText {
		font-size: 1.5rem;
		padding-left: 2.5%;
		font-family: 'IM Fell French Canon SC', serif !important;
		font-weight: 300;
		font-style: normal;
	}

	.Pautas {
		height: 50dvw;
		width: 100vw;
		background: rgb(14 68 109);
		background-repeat: repeat-x;
		background-position: center;
		position: relative;
		height: fit-content;
	}
	/* TOPO */
	.DecAfter {
		width: 100%;
		height: 80px !important;

		background-image: url('./images/BluetornPaperSide.png');
		background-repeat: repeat-x;
		background-size: 100vw;
		rotate: 180deg;
	}

	/* BASE */
	.DecBefore {
		width: 100%;
		height: 80px !important;

		background-image: url('./images/BluetornPaperSide.png');
		background-repeat: repeat-x;
		background-size: 100vw;
	}

	.pauta * {
		color: var(--background-Color);
		text-align: center;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	.pauta {
		width: 33%;
		margin-bottom: 0px;
	}
	.pautaTitle::after {
		content: '';
		display: block;
		left: 5% !important;
		width: 90%;
		height: 2px;
		background-color: var(--background-Color);
	}

	@media (max-width: 480px) {
		.SectionTitle {
			font-size: 10vw;
		}
		.Ender {
			height: 10dvh;
			width: 100dvw;
			position: sticky;
			bottom: 0px;
			left: 0px;
			background: linear-gradient(
				to bottom,
				rgba(255, 255, 240, 0) 0%,
				rgba(255, 255, 240, 1) 99%
			); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
		}
	}
	@media (max-width: 1000px) {
		.pauta {
			width: 100% !important;
		}
		section {
			height: max-content !important;
		}
	}
	@media (max-width: 1665px) {
		.pauta {
			width: 50%;
		}
	}
</style>
