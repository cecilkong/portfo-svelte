<svelte:head>
	<title>Home</title>
	<meta name="description" content="Home Page" />
</svelte:head>

<script lang>
	import ProjectThumbnail from '../components/ProjectThumbnail.svelte'
	import mango from '$lib/images/projects/mango.png'
    import gma_green from '$lib/images/projects/gma-green.png'
    import shade_shift from '$lib/images/projects/shade-shift.png'
    import saleblazers from '$lib/images/projects/saleblazers.png'
	import scare_crow from '$lib/images/projects/sc1.png'
	import bf from '$lib/images/projects/bf-concept.jpeg'

	import mango_gif from '$lib/images/mgms/kpop-hitnotes.gif'
    import gma_green_gif from '$lib/images/gg/plants-1.png'
    import shade_shift_gif from '$lib/images/ss/purple.gif'
    import saleblazers_gif from '$lib/images/sb/environments.gif'
	import scare_crow_gif from '$lib/images/projects/scare-crow.png'
    // import equinox from '$lib/images/projects/equinox.png'
    // import lechord from '$lib/images/projects/lechord.png'
</script>

<div class="intro">
	<!-- <p class="name">
		hi, i'm cecil.
	</p> -->
	<!-- <p class="brief">
		gameplay programmer <br/>
		software engineer <br/>
		artist <br/>
		computer science games @ USC
	</p> -->
</div>

<div class="projects">
	<div class="thumbnail">
		<ProjectThumbnail 
			image={scare_crow}
			gif={scare_crow_gif}
			title="Scare Crow" 
			role="Gameplay Programmer" 
			tools="Unity/C#"
			time="May 2024 - Current" 
			page_link="/projects/scare-crow"
		/>
	</div>
	<div class="thumbnail">
		<ProjectThumbnail
			image={bf} 
			gif={bf}
			title="Tools Programming on Battlefield" 
			role="Software Engineer Intern @ Ripple Effect Studios" 
			tools="Python, C#"
			time="May 2024 - August 2024"
			page_link="/projects/res"
		/>
	</div>
	<div class="thumbnail">
		<ProjectThumbnail
			image={mango} 
			gif={mango_gif}
			title="Mango Goes To Mewsic School" 
			role="Co-Developer" 
			tools="Unity/C#"
			time="January 2023 - June 2023"
			page_link="/projects/mango"
		/>
	</div>
	<div class="thumbnail">
		<ProjectThumbnail 
			image={saleblazers} 
			gif={saleblazers_gif}
			title="Saleblazers" 
			role="Gameplay Programming Intern @ Airstrafe Interactive" 
			tools="Unity/C#"
			time="May 2023 - August 2023"
			page_link="/projects/saleblazers"
		/>
	</div>
	<div class="thumbnail">
		<ProjectThumbnail 
			image={gma_green} 
			gif={gma_green_gif}
			title="Grandma Green" 
			role="Concept Artist, UI Artist" 
			tools="Clip Studio Paint"
			time="June 2022 - June 2023"
			page_link="/projects/grandma-green"
		/>
	</div>
	<div class="thumbnail">
		<ProjectThumbnail 
			image={shade_shift} 
			gif={shade_shift_gif}
			title="Shade Shift"
			role="Programmer, Designer"
			tools="Unity/C#"
			time="July 2022"
			page_link="/projects/shade-shift"
		/>
	</div>
</div>


<style>
	.intro {
		margin: 2vh 0vw 2vh 0vw;
	}

	/* .name {
		margin: 0vh 0vw 5vh 0vw;
		font-weight: 900;
		font-size: 105%;
	} 
	*/

	/* .brief {
		font-weight: 100;
		font-size: 100%;
	} */

	.projects 
	{
		margin-top: 9%;
	}

	.thumbnail {
		margin: 2% 0% 2% 0%;
	}

	:global(body) {
		background-color: #F1F1F1;
		color: #131316;
		transition: background-color 0.3s;
	}

	:global(body.dark-mode) {
		background-color: #131316;
		color: #F1F1F1;
		transition: background-color 0.3s;
	}
</style>
