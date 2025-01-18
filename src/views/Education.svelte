<script>
  // No script needed for static content, but you can add dynamic behavior here if needed.
</script>

<main class="education">
  <h1>Education</h1>

  <section class="education-entry">
    <h3>2019-2023: Florida Institute of Technology</h3>
    <p class="degree">Bachelor of Science (BSc.), Computer Science (Cybersecurity concentration) - Magna Cum Laude</p>
  </section>

  <!-- Moved "Currently Working On" section here -->
  <section class="education-entry">
    <h3>Currently Working On</h3>
    <ul class="subjects-list">
      <li class="subject"><strong>AWS Cloud Practitioner – Foundational Certification</strong>: Studying core AWS services, cloud computing principles, and best practices.</li>
      <li class="subject"><strong>AWS Certified Developer – Associate</strong>: Learning cloud development principles, AWS SDKs, and automation with AWS Lambda.</li>
    </ul>
  </section>

  <section class="education-entry">
    <h3>2016-2018: Bishop Anstey Trinity College East Sixth Form</h3>
    <p class="degree">Open Scholarship Award Winner</p>
    <p class="degree">CAPE Regional Merit List (8th in Caribbean)</p>
    <ul class="subjects-list">
      <li class="subject">CAPE Information Technology Unit 1 - Grade I (Merit)</li>
      <li class="subject">CAPE Information Technology Unit 2 - Grade I</li>
      <li class="subject">CAPE Computer Science Unit 1 - Grade I</li>
      <li class="subject">CAPE Computer Science Unit 2 - Grade I</li>
      <li class="subject">CAPE Pure Mathematics Unit 1 - Grade I</li>
      <li class="subject">CAPE Pure Mathematics Unit 2 - Grade I</li>
      <li class="subject">CAPE Communication Studies - Grade I</li>
      <li class="subject">CAPE Caribbean Studies - Grade I</li>
    </ul>
  </section>

  <section class="education-entry">
    <h3>2011-2016: Holy Cross College</h3>
    <ul class="subjects-list">
      <li class="subject">CSEC Information Technology - Grade I</li>
      <li class="subject">CSEC Principles of Accounts - Grade I</li>
      <li class="subject">CSEC Principles of Business - Grade I (Merit)</li>
      <li class="subject">CSEC Mathematics - Grade I</li>
      <li class="subject">CSEC Additional Mathematics - Grade I</li>
      <li class="subject">CSEC English A - Grade I</li>
      <li class="subject">CSEC Human and Social Biology - Grade I</li>
      <li class="subject">CSEC Theatre Arts - Grade I</li>
    </ul>
  </section>

</main>

<style>
  /* styles for education section */
  .education {
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

  .education-entry {
    margin-bottom: 30px;
    border-left: 4px solid #6c6e70;
    padding-left: 20px;
    background-color: #ffffff;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    transition: background-color 0.3s ease, transform 0.3s ease;
  }

  .education-entry h3 {
    font-size: 1.8rem;
    color: #333;
    margin-bottom: 15px;
  }

  .degree {
    font-size: 1.2rem;
    font-weight: bold;
    color: #555;
    margin-bottom: 10px;
  }

  .subjects-list {
    list-style-type: none; /* Remove bullet points */
    padding-left: 0; /* Remove left padding */
  }

  .subject {
    font-size: 1rem;
    color: #333;
    margin: 5px 0;
  }

  /* Add a subtle hover effect on each entry */
  .education-entry:hover {
    background-color: #f1f1f1;
    transform: translateX(10px);
  }

  /* Mobile responsiveness */
  @media (max-width: 768px) {
    .education {
      padding: 15px;
    }

    h1 {
      font-size: 2rem;
    }

    h2 {
      font-size: 1.8rem;
    }

    h3 {
      font-size: 1.4rem;
    }

    .degree {
      font-size: 1rem;
    }

    .subject {
      font-size: 0.95rem;
    }
  }

  @media (max-width: 480px) {
    h1 {
      font-size: 1.8rem;
    }

    h2 {
      font-size: 1.6rem;
    }

    h3 {
      font-size: 1.2rem;
    }

    .degree {
      font-size: 0.9rem;
    }

    .subject {
      font-size: 0.85rem;
    }
  }
</style>
