<script>
	import { slide } from 'svelte/transition'; // Import the slide transition from Svelte
	import { onMount } from 'svelte';
	import Header from './components/Header.svelte';
	import Home from './views/Home.svelte';
	import WorkExperience from './views/WorkExperience.svelte';
	import Education from './views/Education.svelte';
	import Projects from './views/Projects.svelte';
	import Skills from './views/Skills.svelte';
    import Overview from './views/Overview.svelte';
  
	let selectedSection = 'home'; // Default selected section
  
	// Function to handle navigation changes
	function changeSection(section) {
	  selectedSection = section;
	}
  </script>
  
  <Header {changeSection} />
  <main class="content">
	{#if selectedSection === 'home'}
	  <div class="section-wrapper" transition:slide={{ duration: 500, x: 300 }}>
		<Home />
	  </div>
	{:else if selectedSection === 'overview'}
	<div class="section-wrapper" transition:slide={{ duration: 500, x: 300 }}>
	<Overview />
	  </div>
	{:else if selectedSection === 'workExperience'}
	  <div class="section-wrapper" transition:slide={{ duration: 500, x: 300 }}>
		<WorkExperience />
	  </div>
	{:else if selectedSection === 'education'}
	  <div class="section-wrapper" transition:slide={{ duration: 500, x: 300 }}>
		<Education />
	  </div>
	{:else if selectedSection === 'projects'}
	  <div class="section-wrapper" transition:slide={{ duration: 500, x: 300 }}>
		<Projects />
	  </div>
	{:else if selectedSection === 'skills'}
	  <div class="section-wrapper" transition:slide={{ duration: 500, x: 300 }}>
		<Skills />
	  </div>
	{/if}
  </main>
  
  <style>
	/* Ensure content starts below the header */
	.content {
	  margin-top: 30px; /* Match the height of the header to prevent overlap */
	  padding: 30px; /* Optional: padding for inner spacing of the sections */
	}
  
	.section-wrapper {
	  /* Optional: any styling for the wrapper */
	}
  </style>
  