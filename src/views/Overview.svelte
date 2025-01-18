<script>
  // No script needed for now
</script>

<main class="home">
  <h1>Jerrel Gordon</h1>
  <h3>DevOps Software Engineer</h3>

  <!-- Technical Summary Section -->
  <section class="home-category">
    <h2>Technical Summary</h2>
    <p>
      I’ve worked in the food and beverage industry, building and maintaining inventory control systems for a major manufacturer. In this role, I collaborated closely with users and stakeholders to ensure smooth processes from design through implementation and support.
    </p>
    <p>
      I also have research experience with Raspberry Pi, testing DNS server security in an NFV/SDN setup. This is where I first got into cloud computing through CloudStack, which inspired me to dive deeper into the cloud. I’m currently working towards AWS Solutions Architect and AWS Developer Associate certifications to build on that knowledge.
    </p>
    <p>
      For more details on my skills, work experience, and projects, check out the <strong>Skills</strong>, <strong>Work Experience</strong>, and <strong>Projects</strong> sections in my Cloud Resume Challenge. Just click the hamburger icon in the top-right corner to explore!
    </p>
  </section>

  <!-- Cloud Resume Challenge Section -->
  <section class="home-category">
    <h2>My Cloud Resume Challenge</h2>
    <p>
      ... in progress
    </p>
  </section>

  <!-- Technical Breakdown from Developer's Perspective -->
  <section class="home-category">
    <h2>Technical Breakdown: Developer</h2>
    <p>
      ... in progress
    </p>
    <!-- Diagram for Developer's Perspective -->
    <div class="diagram">
      <h3>Developer's Architecture Overview</h3>
      <img src="../assets/dev-flow.png" alt="Developer's Architecture Diagram" />
    </div>
  </section>

  <!-- Technical Breakdown from User's Perspective -->
  <section class="home-category">
    <h2>Technical Breakdown: User</h2>
    <p>
      ... in progress
    </p>
    <!-- Diagram for User's Perspective -->
    <div class="diagram">
      <h3>User Experience Flow</h3>
      <img src="../assets/user-flow.png" alt="User's Perspective Diagram" />
    </div>
  </section>

  <!-- Thank You Section -->
  <section class="home-category">
    <h2>Thanks for Visiting!</h2>
    <p>
      ... in progress
    </p>
  </section>
</main>

<style>
  /* General styles for the home section */
  .home {
    padding: 20px;
    max-width: 900px;
    margin: 0 auto;
    background-color: #383838;
    border-radius: 8px;
    color: #dddddd; /* Light text color */
  }

  h1 {
    font-size: 2.5rem;
    color: #dddddd;
    font-weight: bold;
  }

  h3 {
    font-size: 1.5rem;
    color: #979797;
    font-weight: bold;
  }

  /* Skill category section box styles */
  .home-category {
    background-color: #ffffff;
    padding: 20px;
    margin-bottom: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    text-align: left;
    transition: background-color 0.3s ease;
  }

  .home-category h2 {
    font-size: 1.8rem;
    color: #333;
    margin-bottom: 10px;
  }

  .home-category p {
    font-size: 1.1rem;
    line-height: 1.6;
    color: #555;
  }

  .diagram {
    margin-top: 20px;
    text-align: center;
  }

  .diagram img {
    width: 100%;
    max-width: 800px;
    height: auto;
  }

  .diagram h3 {
    font-size: 1.4rem;
    color: #333;
    margin-bottom: 10px;
  }

  .home-category:hover {
    background-color: #f1f1f1;
  }

  /* Mobile responsiveness */
  @media (max-width: 768px) {
    .home {
      padding: 15px;
    }

    h1 {
      font-size: 2rem;
    }

    h2 {
      font-size: 1.6rem;
    }

    .home-category h2 {
      font-size: 1.4rem;
    }

    .home-category p {
      font-size: 1rem;
    }

    .diagram h3 {
      font-size: 1.2rem;
    }
  }

  @media (max-width: 480px) {
    h1 {
      font-size: 1.8rem;
    }

    h2 {
      font-size: 1.6rem;
    }

    .home-category h2 {
      font-size: 1.2rem;
    }

    .home-category p {
      font-size: 0.9rem;
    }

    .diagram img {
      width: 100%;
      max-width: 100%;
    }
  }
</style>
