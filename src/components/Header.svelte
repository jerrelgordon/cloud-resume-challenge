<script>
  import { fade } from 'svelte/transition';
  import VisitorCount from './VisitorCount.svelte';
  export let changeSection;
  let menuOpen = false;
  let isPulsing = true; // Track whether the pulsing animation should be active

  // Close the menu when clicking outside of it
  const closeMenuIfClickedOutside = (event) => {
    const menu = document.querySelector('.nav-menu');
    const hamburger = document.querySelector('.hamburger');
    if (menu && !menu.contains(event.target) && !hamburger.contains(event.target)) {
      menuOpen = false;
    }
  };

  import { onMount, onDestroy } from 'svelte';
  onMount(() => {
    document.addEventListener('click', closeMenuIfClickedOutside);

    setTimeout(() => {
      isPulsing = false;
    }, 3000); // Stop pulsing after 3 seconds
  });

  onDestroy(() => {
    document.removeEventListener('click', closeMenuIfClickedOutside);
  });

  
</script>

<header>
  <div class="left">
    <VisitorCount />
  </div>
  <button class="hamburger" on:click={() => menuOpen = !menuOpen} class:active={isPulsing}>
    ☰
  </button>
  {#if menuOpen}
    <nav class="nav-menu" transition:fade={{ duration: 300 }}>
      <a href="#" on:click={() => { changeSection('home'); menuOpen = false; }}>Home</a>
      <a href="#" on:click={() => { changeSection('overview'); menuOpen = false; }}>Overview</a>
      <a href="#" on:click={() => { changeSection('workExperience'); menuOpen = false; }}>Work Experience</a>
      <a href="#" on:click={() => { changeSection('education'); menuOpen = false; }}>Education</a>
      <a href="#" on:click={() => { changeSection('projects'); menuOpen = false; }}>Projects</a>
      <a href="#" on:click={() => { changeSection('skills'); menuOpen = false; }}>Skills</a>
    </nav>
  {/if}
</header>

<style>
  /* Styling for the entire header */
  header {
    display: flex;
    justify-content: space-between; /* Space out the elements */
    align-items: center;
    background-color: #333;
    color: white;
    padding: 10px 20px;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 10;
    height: 60px; 
  }

  /* Styling for the left part of the header */
  .left {
    font-size: 1.2rem;
  }

  /* Styling for the hamburger button */
  .hamburger {
    font-size: 2rem;
    background: none;
    border: none;
    color: white;
    cursor: pointer;
    transition: transform 0.3s ease;
  }

  /* More noticeable pulsing animation when the hamburger button is active */
  .hamburger.active {
    animation: pulse 0.6s ease-in-out infinite; /* Faster animation with noticeable pulse */
  }

  @keyframes pulse {
    0% {
      transform: scale(1);
    }
    50% {
      transform: scale(1.2); /* Larger scale for more obvious pulsing */
    }
    100% {
      transform: scale(1);
    }
  }

  /* Styling for the navigation menu */
  .nav-menu {
    display: flex;
    flex-direction: column;
    position: absolute;
    top: 60px; /* Position below the header */
    right: 10px; 
    background-color: #333;
    padding: 10px;
    border-radius: 8px;
  }

  .nav-menu a {
    text-decoration: none;
    margin: 10px 0;
    color: white;
    font-size: 1.2rem;
  }

  .nav-menu a:hover {
    text-decoration: underline;
  }

  /* Mobile responsive design */
  @media (max-width: 768px) {
    header {
      padding: 10px 15px;
      flex-direction: row; /* Horizontal layout */
      justify-content: space-between; /* Ensure space between items */
    }

    .left {
      font-size: 1.1rem;
      margin-right: auto; /* Push the hamburger button to the far right */
    }

    .hamburger {
      font-size: 2.5rem;
      margin-left: auto; /* Align hamburger to the far right */
    }

    .nav-menu {
      top: 60px; /* Ensure it opens below the header */
      right: 0;
      padding: 15px;
      border-radius: 8px;
    }

    .nav-menu a {
      font-size: 1.5rem;
    }
  }

  /* For very small screens (mobile-first adjustments) */
  @media (max-width: 480px) {
    header {
      padding: 8px 10px;
    }

    .left {
      font-size: 1rem;
    }

    .hamburger {
      font-size: 3rem;
    }

    .nav-menu {
      padding: 20px;
    }

    .nav-menu a {
      font-size: 1.4rem;
    }
  }
</style>
