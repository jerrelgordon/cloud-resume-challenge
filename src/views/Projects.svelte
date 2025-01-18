<script>
  // No script needed for now
</script>

<main class="projects">
  <h1>Projects</h1>

  <section class="project-entry">
    <h3>Metasploit Module</h3>
    <p class="project-description">Developed a specialized module for the open-source Metasploit framework, enabling users to seamlessly retrieve bookmarks on the target machine post-exploitation.</p>
    <p class="project-description">Tailored for Chrome, Edge, Explorer, and Opera browsers.</p>
  </section>

  <section class="project-entry">
    <h3>Autonomous Exploit Generator</h3>
    <p class="project-description">Collaborated with a reverse engineering team developing a tool for discovering and exploiting vulnerabilities.</p>
    <p class="project-description">Utilized techniques like return-oriented programming, format strings, and symbolic execution.</p>
  </section>

  <section class="project-entry">
    <h3>Windows Keylogger (Stealthy)</h3>
    <p class="project-description">Implemented MITRE ATT&CK Framework concepts to create a stealthy keylogger.</p>
    <p class="project-description">Evasion of virus detection, persistence establishment, and program partitioning/assembly execution.</p>
    <p class="project-description">Currently expanding functionality to support arbitrary command execution.</p>
  </section>

  <section class="project-entry">
    <h3>Cloud Resume Challenge</h3>
    <p class="project-description">****In Progress****</p>
  </section>

</main>

<style>
  /* General styles for the projects section */
  .projects {
    padding: 20px;
    max-width: 900px;
    margin: 0 auto;
    background-color: #383838;
    border-radius: 8px;
    color: #dddddd; /* Light text color */
  }

  h1 {
    font-size: 2.5rem;
    margin-bottom: 20px;
    color: #dddddd;
    font-weight: bold;
  }

  .project-entry {
    margin-bottom: 30px;
    border-left: 4px solid #ccc;
    padding-left: 20px;
    background-color: #ffffff;
    padding: 15px;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    text-align: left;
  }

  .project-entry h3 {
    font-size: 1.8rem;
    color: #333;
    margin-bottom: 10px;
  }

  .project-description {
    font-size: 1.2rem;
    color: #555;
    margin-bottom: 10px;
  }

  .project-entry:hover {
    background-color: #f1f1f1;
  }

  /* Mobile responsiveness */
  @media (max-width: 768px) {
    .projects {
      padding: 15px;
    }

    h1 {
      font-size: 2rem;
    }

    h3 {
      font-size: 1.4rem;
    }

    .project-description {
      font-size: 1rem;
    }
  }

  @media (max-width: 480px) {
    h1 {
      font-size: 1.8rem;
    }

    h3 {
      font-size: 1.2rem;
    }

    .project-description {
      font-size: 0.9rem;
    }
  }
</style>
