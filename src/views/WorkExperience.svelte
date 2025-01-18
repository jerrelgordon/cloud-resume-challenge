<script>
    // No script needed for now
  </script>
  
  <main class="work-experience">
    <h1>Work Experience</h1>
  
    <section class="job">
        <h3>2023 - Present: Computer Task Group (CTG)</h3>
        <p class="position-title">Associate Software Engineer</p>
        <ul>
            <li class="job-description">AGILE environment where our team refactors an Inventory Control System for a US food and beverage company to enhance efficiency.</li>
            <li class="job-description">Specialized in integrating shipping and order management features based on client requirements.</li>
            <li class="job-description">Proficient in creating documentation, including test plans, design docs, deployment notes, and conducting code reviews.</li>
            <li class="job-description">Providing technical support to troubleshoot issues encountered in production.</li>
            <li class="job-description">Work closely with stakeholders to ensure consistent satisfaction before, during, and after product delivery.</li>
        </ul>
    </section>
  
    <section class="job">
        <h3>2022 - 2023: Florida Institute of Technology</h3>
        <p class="position-title">Research Assistant</p>
        <ul>
            <li class="job-description">Implemented diverse DNS servers, incorporating DOT, DOH, and DNSSEC, leveraging NFV/SDN concepts using CloudStack and Ubuntu.</li>
            <li class="job-description">Collaborated on joint research with graduate students at Florida International University, deploying these servers on their 5G testbed.</li>
            <li class="job-description">Conducted experiments to compare and contrast DNS security measures.</li>
        </ul>
    </section>
  
    <section class="job">
        <h3>2021 - 2023: Florida Institute of Technology</h3>
        <p class="position-title">Computer Science Tutor</p>
        <ul>
            <li class="job-description">Mentored undergraduate students in courses including but not limited to: Fundamentals of Programming 1 & 2, Intro to C++, Data Structures and Algorithms, and Operating Systems.</li>
        </ul>
    </section>
  
    <section class="job">
        <h3>2018 - 2019: Grande Law Chambers</h3>
        <p class="position-title">Law Clerk</p>
        <ul>
            <li class="job-description">Assisting attorney with drafting and filing legal documents including:</li>
            <li class="job-description">Family Court</li>
            <li class="job-description">Civil/Petty Civil Court</li>
            <li class="job-description">Land/Deeds</li>
            <li class="job-description">Probate</li>
        </ul>
    </section>
  </main>
  
  <style>
    /* General styles for the work experience section */
    .work-experience {
        padding: 20px;
        max-width: 900px;
        margin: 0 auto;
        background-color: #383838; /* Light grey background */
        border-radius: 8px;
    }
  
    h1 {
        font-size: 2.5rem;
        margin-bottom: 20px;
        color: #dddddd;
        font-weight: bold;
    }
  
    .job {
        margin-bottom: 30px;
        border-left: 4px solid #ccc;
        padding-left: 20px;
        background-color: #ffffff; /* White background for job sections */
        padding: 15px;
        border-radius: 8px;
        box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1); /* Subtle shadow for separation */
        text-align: left; 
        transition: background-color 0.3s ease;
    }
  
    .job h3 {
        font-size: 1.8rem;
        color: #333; 
        margin-bottom: 10px;
    }
  
    .position-title {
        font-size: 1.2rem;
        font-weight: bold;
        color: #555; 
        margin-bottom: 10px;
    }
  
    .job-description {
        font-size: 1rem;
        color: #333;
        margin: 5px 0;
        padding-left: 30px; 
        position: relative;
        text-align: left;
        transition: padding-left 0.3s ease, color 0.3s ease;
    }
  
    /* Remove default bullet points */
    ul {
        list-style-type: none;
        padding-left: 0;
    }
  
    /* Adding arrows to the job description items */
    .job-description::before {
        content: '➤';
        position: absolute;
        left: 0; 
        color: #3ad1f7; 
        font-size: 1.2rem;
        margin-right: 10px;
        top: 0; 
    }
  
    .job-description:hover {
        color: #868686;
        padding-left: 35px; /* Move over slightly when hovered */
    }
  
    .job:hover {
        background-color: #f1f1f1;
    }
  
    /* Mobile responsiveness */
    @media (max-width: 768px) {
        .work-experience {
            padding: 15px;
        }
  
        h1 {
            font-size: 2rem; 
        }
  
        .job {
            padding: 10px;
            margin-bottom: 20px;
        }
  
        .job h3 {
            font-size: 1.5rem;
        }
  
        .position-title {
            font-size: 1rem; 
        }
  
        .job-description {
            font-size: 0.95rem;
            padding-left: 25px; 
        }
    }
  
    @media (max-width: 480px) {
        .job-description {
            font-size: 0.9rem;
            padding-left: 20px;
        }
        
        h1 {
            font-size: 1.8rem;
        }
    }
  </style>
  