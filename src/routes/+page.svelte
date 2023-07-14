<script>
	import { onMount } from 'svelte';
	import { fade, fly } from 'svelte/transition';
	import { flip } from 'svelte/animate';
	import Socials from '../lib/Socials.svelte';
	import Navbar from '../lib/Navbar.svelte';
</script>

<main>
	<!-- <Navbar /> -->
	<div class="container">
		<div class="heading-container">
			<h1>
				Hey, I am <span class="highlight">Akshat.</span>
			</h1>
		</div>

		<p>
			I am a computer science engineer dedicated to tackling the world's most formidable challenges by
			translating promising laboratory ideas into impactful real-world solutions. With expertise in computer 
            science and electronics, including artificial intelligence, autonomous technologies, scalable computing, 
            and fintech, I strive to make a meaningful impact by inventing next-gen technologies.
		</p>

		<p>
			If you are an innovative thinker or share my passion for leveraging technology as a catalyst for positive change, 
            I would love to to connect with you. Whether you have groundbreaking problem-solving ideas or simply seek engaging 
            discussions, I am enthusiastic about collaborating and exploring new possibilities. Please feel free to reach out to 
            me at  <a href="mailto:akshatk163@gmail.com">akshatk163@gmail.com</a>.
		</p>

		<Socials />
	</div>
</main>

<style>
	.container {
		max-width: 100%;
		padding: 0 1rem;
	}

	.heading-container {
		display: flex;
		justify-content: center;
		margin-top: 5vh;
		margin-bottom: 1rem;
	}

	h1 {
		font-family: 'Roboto', sans-serif;
		font-weight: 400;
		font-size: 2rem;
		letter-spacing: -0.015em;
		text-align: center;
		line-height: 1.2;
		margin: 0;
		padding: 1rem 0;
		position: relative;
	}

	h1::before,
	h1::after {
		content: '';
		display: block;
		width: 30%;
		height: 1px;
		position: absolute;
		top: 50%;
		transform: translateY(-50%);
		background-color: white;
	}

	h1::before {
		left: -35%;
	}

	h1::after {
		right: -35%;
	}

	.highlight {
		color: #a660ff;
		text-shadow: 0px 0px 15px rgba(166, 96, 255, 0.5);
	}

	p {
		font-family: 'Roboto';
		font-style: normal;
		font-weight: 300;
		font-size: 1.2rem;
		line-height: 1.8rem;
		letter-spacing: -0.015em;
		text-align: center;
		color: #c8c8c8;
		margin: 1.5rem auto;
		max-width: 70ch;
	}

	a {
		color: white;
	}

	/* media query */
	@media (max-width: 768px) {
		h1 {
			font-size: 2.8rem;
		}

		p {
			font-size: 1.2rem;
			line-height: 1.8rem;
		}
	}
</style>
