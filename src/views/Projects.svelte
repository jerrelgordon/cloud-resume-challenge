<script>
  // No script needed for now
</script>

<main class="projects">
  <h1>Projects</h1>

  <section class="project-entry">
    <h3>Cloud Resume Challenge</h3>
    <div class="project-details">
      <div class="detail">
        <strong>GitHub Link:</strong> 
        <a href="https://github.com/jerrelgordon/cloud-resume-challenge" target="_blank">AWS Cloud Resume Challenge Repository</a>
      </div>
      <div class="detail">
        <strong>Tools Used:</strong> 
        <p>Svelte, Cloudfront, S3, Lambda, APIGateway, DynamoDB, Route53, ACM, IAM, GitHub Actions</p>
      </div>
      <div class="detail">
        <strong>Project Summary:</strong> 
        <p>Built a state-driven, single-page web app with the Svelte framework, utilizing AWS cloud services such as S3 for static hosting, Cloudfront for distribution, Lambda and APIGateway for serverless functionality. Set up a CI/CD pipeline using GitHub Actions coupled with a secure AWS IAM user.</p>
      </div>
    </div>
  </section>

  <section class="project-entry">
    <h3>Metasploit Module</h3>
    <div class="project-details">
      <div class="detail">
        <strong>GitHub Link:</strong> 
        <a href="https://github.com/jerrelgordon/metasploit-get-bookmarks-module" target="_blank">MetaSploit: Get_Bookmarks.rb</a>
      </div>
      <div class="detail">
        <strong>Tools Used:</strong> 
        <p>Ruby</p>
      </div>
      <div class="detail">
        <strong>Project Summary:</strong> 
        <p>Developed a specialized module for the open-source Metasploit framework, enabling users to seamlessly retrieve bookmarks on the target machine post-exploitation. Tailored for Chrome, Edge, Explorer, and Opera browsers.</p>
      </div>
    </div>
  </section>

  <section class="project-entry">
    <h3>Autonomous Exploit Generator</h3>
    <div class="project-details">
      <div class="detail">
        <strong>GitHub Link:</strong> 
        <a href="https://github.com/jerrelgordon" target="_blank">Jerrel's Github</a>
      </div>
      <div class="detail">
        <strong>Tools Used:</strong> 
        <p>Binary Ninja, Python</p>
      </div>
      <div class="detail">
        <strong>Project Summary:</strong> 
        <p>Collaborated with a reverse engineering team to develop a tool for discovering and exploiting vulnerabilities. Utilized techniques like return-oriented programming, format strings, and symbolic execution to generate autonomous exploits.</p>
      </div>
    </div>
  </section>

  <section class="project-entry">
    <h3>Windows Keylogger (Stealthy)</h3>
    <div class="project-details">
      <div class="detail">
        <strong>GitHub Link:</strong> 
        <a href="https://github.com/jerrelgordon" target="_blank">Jerrel's Github</a>
      </div>
      <div class="detail">
        <strong>Tools Used:</strong> 
        <p>C, Python</p>
      </div>
      <div class="detail">
        <strong>Project Summary:</strong> 
        <p>Implemented MITRE ATT&CK Framework concepts to create a stealthy keylogger with evasion techniques for virus detection and persistence establishment. Currently expanding functionality to support arbitrary command execution and more sophisticated evasion methods.</p>
      </div>
    </div>
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
    color: #dddddd;
  }

  h1 {
    font-size: 2.5rem;
    margin-bottom: 20px;
    color: #dddddd;
    font-weight: bold;
  }

  .project-entry {
    margin-bottom: 30px;
    border-left: 4px solid #8a8a8a;
    padding-left: 20px;
    background-color: #ffffff;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    transition: background-color 0.3s ease, transform 0.3s ease;
  }

  .project-entry h3 {
    font-size: 1.8rem;
    color: #333;
    margin-bottom: 15px;
  }

  .project-details {
    margin-left: 20px;
  }

  .detail {
    font-size: 1.1rem;
    color: #555;
    margin-bottom: 15px;
  }

  .detail strong {
    color: #333;
    font-weight: bold;
  }

  .detail a {
    color: #2b81b3;
    text-decoration: none;
    transition: color 0.3s ease;
  }

  .detail a:hover {
    color: #333;
  }

  .project-entry:hover {
    background-color: #f9f9f9;
    transform: translateX(10px);
  }

  /* Mobile responsiveness */
  @media (max-width: 768px) {
    .projects {
      padding: 15px;
    }

    h1 {
      font-size: 2rem;
    }

    .project-entry {
      padding: 15px;
      margin-bottom: 20px;
    }

    .project-entry h3 {
      font-size: 1.6rem;
    }

    .detail {
      font-size: 1rem;
    }
  }

  @media (max-width: 480px) {
    h1 {
      font-size: 1.8rem;
    }

    .project-entry h3 {
      font-size: 1.4rem;
    }

    .detail {
      font-size: 0.9rem;
    }
  }
</style>
