<script>
	import { goto } from '$app/navigation';
	import { onMount } from 'svelte';

	let ScreenWidth = 1080;

	onMount(() => {});
</script>

<div class="MainContainer">
	<section class="titleSection">
		<h1>Gremio Estudantil Arnaldo Cardoso Rocha</h1>
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
		{#if ScreenWidth > 768}
			<div class="Pautas"></div>
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
	@import url('https://fonts.googleapis.com/css2?family=IM+Fell+French+Canon:ital@0;1&family=Ubuntu:ital,wght@0,300;0,400;0,500;0,700;1,300;1,400;1,500;1,700&display=swap');

	section {
		width: 100dvw;
		height: max-content;
		margin-bottom: 5dvh;
	}
	.titleSection {
		width: 100dvw;
		background: url('./images/Tarifa0.webp');
		height: 50dvh;
		display: flex;
		align-items: center;
		justify-content: center;
	}
	.TextContainer {
		width: 80%;
		margin: 0 auto;
	}
	.SectionTitle {
		color: var(--Red-Accent);
		font-size: 4rem;
	}
	.MinorText {
		font-size: 1.5rem;
		padding-left: 2.5%;
		font-family: 'Ubuntu', sans-serif !important;
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
		height: 70dvh;
		width: 100dvw;
		background: url('./images/G1Blue.png');
		background-repeat: no-repeat;
		background-size: contain;
	}
</style>
