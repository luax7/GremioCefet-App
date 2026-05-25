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
			<div class="Pautas"></div>
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
		height: max-content;
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
	.Ender {
		height: 10dvh;
		width: 100dvw;
		position: sticky;
		bottom: 0px;
		left: 0px;
		background: linear-gradient(
			to bottom,
			rgba(255, 255, 240, 0) 0%,
			rgba(255, 255, 240, 0) 3%,
			rgba(255, 255, 240, 1) 53%,
			rgba(255, 255, 240, 1) 99%
		); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
	}
	.Pautas {
		height: 50dvw;
		width: 100vw;
		background: rgb(14 68 109);
		background-repeat: repeat-x;
		background-position: center;
		position: relative;
	}
	/* TOPO */
	.DecAfter {
		width: 100%;
		height: 80px;

		background-image: url('./images/BluetornPaperSide.png');
		background-repeat: repeat-x;
		background-size: auto 100%;
		rotate: 180deg;
	}

	/* BASE */
	.DecBefore {
		width: 100%;
		height: 80px;

		background-image: url('./images/BluetornPaperSide.png');
		background-repeat: repeat-x;
		background-size: auto 100%;
	}
</style>
