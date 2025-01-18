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
      Hello! I'm Jerrel Gordon, a Software Engineer with a background in Control Systems within the manufacturing industry. I studied Computer Science at the Florida Institute of Technology, graduating magna cum laude. 
      During my time there, I served as president of Upsilon Pi Epsilon, the Computer Science honor society. My concentration was in Cybersecurity, and I focused on research involving DNS (DOH, DOT, DNSSEC), comparing 
      security and efficiency using NFV and SDN concepts, while leveraging OpenStack for implementation. This research ignited my passion for Cloud Computing, leading me to dive deeper into AWS services and cloud architecture.
    </p>
    <p>
      For more details on my skills, work experience, and projects, check out the <strong>Skills</strong>, <strong>Work Experience</strong>, and <strong>Projects</strong> sections in my Cloud Resume Challenge. Just click the hamburger icon in the top-right corner to explore!
    </p>
  </section>

  <!-- Cloud Resume Challenge Section -->
  <section class="home-category">
    <h2>My Cloud Resume Challenge</h2>
    <p>
      This project is a state-driven single-page web app built with the Svelte framework, integrating several AWS services such as S3, CloudFront, Route 53, ACM, IAM, Lambda, API Gateway, and DynamoDB. 
      The goal is to create a dynamic, serverless web app that showcases my cloud resume, all while leveraging modern web technologies and AWS services.
      I didn’t always find web development exciting. Early on, I was more focused on other areas of tech. But then, in a random Reddit thread, I stumbled upon Svelte, a lightweight and modern framework. 
      Intrigued by its simplicity and performance, I decided to give it a try. At the same time, I was diving deeper into cloud computing, studying for the AWS Solutions Architect and AWS Associate Developer certifications. 
      This project was the perfect opportunity to merge both my web development skills and cloud knowledge into one fun, practical challenge!
    </p>
  </section>

  <!-- Technical Breakdown from Developer's Perspective -->
  <section class="home-category">
    <h2>Backend: AWS Services</h2>
    <p>To power the app’s backend, I leveraged various AWS services:</p>
    <ul class="service-list">
      <li>S3: Hosts the build artifacts of my Svelte app.</li>
      <li>CloudFront: Serves the content via a CDN for fast global access.</li>
      <li>Route 53: Manages DNS for the custom domain and directs traffic to S3 and CloudFront.</li>
      <li>ACM: Provides an SSL certificate for secure HTTPS connections.</li>
      <li>IAM: Used to create a github user for managing programmatic access.</li>
      <li>DynamoDB: Keeps track of the number of visits my webapp has gotten.</li>
      <li>Lambda & API Gateway: Handles serverless functions for updating the visitor count.</li>
    </ul>
    <p>These services work together to make the app fully functional, scalable, and secure.</p>

    <!-- Diagram for Developer's Perspective -->
    <div class="diagram">
      <h3>Developer's Architecture Overview</h3>
      <img src="../assets/dev-flow.png" alt="Developer's Architecture Diagram" />
    </div>
  </section>

  <!-- Frontend: Svelte Framework -->
  <section class="home-category">
    <h2>Frontend: Svelte Framework</h2>
    <p>Svelte was the ideal choice for this project because it:</p>
    <ul class="service-list">
      <li>Compiles to efficient JavaScript: The build output is small and fast.</li>
      <li>Uses reactive state management: Makes it easy to create dynamic, state-driven components.</li>
      <li>Offers a simple developer experience: The syntax is clean, and setup is straightforward, allowing me to focus on building the app rather than fighting the framework.</li>
    </ul>
    <p>The frontend displays my cloud resume in a clean, user-friendly web app, with data pulled from AWS services like DynamoDB.</p>

    <!-- Diagram for User's Perspective -->
    <div class="diagram">
      <h3>User Experience Flow</h3>
      <img src="../assets/user-flow.png" alt="User's Perspective Diagram" />
    </div>

    <h3>CI/CD Pipeline with GitHub Actions</h3>
    <p>To automate deployments, I set up a CI/CD pipeline using GitHub Actions. Here's how it works:</p>
    <ul class="service-list">
      <li>GitHub Actions is triggered every time I push to the `main` branch.</li>
      <li>It installs the project dependencies, runs `npm run build` to generate static files, and syncs the build output to the S3 bucket.</li>
      <li>It then invalidates the CloudFront cache to ensure the latest version of the app is served.</li>
    </ul>
    <p>This pipeline ensures that the app is always up to date, and I don’t have to manually deploy changes every time.</p>

    <h3>Secrets and Security</h3>
    <p>To keep my AWS credentials safe, I store sensitive data like AWS_ACCESS_KEY_ID, AWS_SECRET_ACCESS_KEY, CLOUDFRONT_DISTRIBUTION_ID and the S3_BUCKET_NAME in GitHub Secrets. This prevents accidental exposure of credentials in the codebase.</p>
  </section>

  <!-- Thank You Section -->
  <section class="home-category">
    <h2>Thanks for Visiting!</h2>
    <p>
      This project has been a great way to combine my growing skills in web development and cloud computing. By building and deploying a serverless web app, I’ve gained hands-on experience 
      with key AWS services and learned how to automate deployments with GitHub Actions. I’m excited to see where this cloud stuff takes me :)
      Thanks for checking out my Cloud Resume Challenge project! 🌐🚀
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

  /* Styling for the list of services */
  .service-list {
    font-size: 1.1rem;
    line-height: 1.7;
    color: #444;
    margin-left: 20px;
    padding: 0;
    list-style: none; /* Remove default list bullets */
  }

  .service-list li {
    margin-bottom: 12px;
    padding-left: 20px; /* Added space for the arrow */
    position: relative;
    transition: color 0.2s ease, padding-left 0.2s ease;
  }

  .service-list li::before {
    content: '➤';
    position: absolute;
    left: 0;
    color: #3ad1f7;
  }

  .service-list li:hover {
    color: #868686;
    padding-left: 25px; /* Move over slightly when hovered */
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
