<script>
  // No script needed for now
</script>

<main class="skills">
  <h1>Skills</h1>
  <p>A list of some of the cool stuff I've learned over the years, including but not limited to: programming languages, frameworks, OS, and cloud technologies. Feel free to reach out to me if you wanna geek out over any of them! Either I can learn something from you or vice versa. :)</p>

  <section class="skills-category">
    <h2>Programming Languages</h2>
    <ul>
      <li>C# (.NET 6, 7, 8), Blazor</li>
      <li>Python</li>
      <li>JavaScript / Node.js</li>
      <li>C / C++</li>
      <li>Rust</li>
      <li>Ruby</li>
      <li>HTML / CSS</li>
    </ul>
  </section>

  <section class="skills-category">
    <h2>Web Development & Frameworks</h2>
    <ul>
      <li>Blazor (C#)</li>
      <li>RESTful APIs</li>
      <li>Node.js (JavaScript)</li>
      <li>WordPress</li>
    </ul>
  </section>

  <section class="skills-category">
    <h2>Database Technologies</h2>
    <ul>
      <li>PostgreSQL</li>
      <li>DynamoDB</li>
    </ul>
  </section>

  <section class="skills-category">
    <h2>Cloud & AWS Services</h2>
    <ul>
      <li>AWS Simple Storage Service (S3)</li>
      <li>AWS Elastic Compute Cloud (EC2)</li>
      <li>AWS CloudFront (CDN)</li>
      <li>AWS CloudWatch</li>
      <li>AWS DynamoDB (NoSQL)</li>
    </ul>
  </section>

  <section class="skills-category">
    <h2>Operating Systems & Platforms</h2>
    <ul>
      <li>Ubuntu</li>
      <li>Kali Linux</li>
      <li>OpenStack (Cloud Infrastructure)</li>
    </ul>
  </section>

  <section class="skills-category">
    <h2>DevOps & Containers</h2>
    <ul>
      <li>Docker</li>
    </ul>
  </section>

  <section class="skills-category">
    <h2>Security & Networking</h2>
    <ul>
      <li>Penetration Testing</li>
      <li>WireShark, NetSpot (Network Traffic Analysis)</li>
      <li>MetaSploit (check out the Module I added! :))</li>
      <li>Autopsy, BinWalk (Memory Forensics)</li>
    </ul>
  </section>
</main>

<style>
  /* styles for the skills section */
  .skills {
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

  /* Skill category section box styles */
  .skills-category {
    background-color: #ffffff;
    padding: 20px;
    margin-bottom: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    text-align: left;
  }

  .skills-category h2 {
    font-size: 1.8rem;
    color: #333;
    margin-bottom: 10px;
  }

  .skills-category ul {
    list-style-type: none; /* Remove bullet points */
    padding-left: 0; /* Remove left padding */
  }

  .skills-category li {
    font-size: 1.2rem;
    color: #555;
    margin: 5px 0;
    padding-left: 30px; /* Add space for the arrow */
    position: relative;
  }

  /* Adding arrows to the list items */
  .skills-category li::before {
    content: '→'; /* Right arrow symbol */
    position: absolute;
    left: 0;
    color: #555;
    font-size: 1.2rem;
    margin-right: 10px;
    top: 0;
  }

  .skills-category:hover {
    background-color: #f1f1f1;
  }

  /* Mobile responsiveness */
  @media (max-width: 768px) {
    .skills {
      padding: 15px;
    }

    h1 {
      font-size: 2rem;
    }

    h2 {
      font-size: 1.6rem;
    }

    .skills-category h2 {
      font-size: 1.4rem;
    }

    .skills-category li {
      font-size: 1rem;
    }
  }

  @media (max-width: 480px) {
    h1 {
      font-size: 1.8rem;
    }

    h2 {
      font-size: 1.6rem;
    }

    .skills-category h2 {
      font-size: 1.2rem;
    }

    .skills-category li {
      font-size: 0.95rem;
    }
  }
</style>
