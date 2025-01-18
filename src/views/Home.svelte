<script>
    // Define the URLs for the social media pages - youtube link will be updated to a channel where I do video explanations
    const githubUrl = 'https://www.github.com/jerrelgordon/';
    const linkedinUrl = 'https://www.linkedin.com/in/jerrel-gordon-131ba5111';
    const youtubeUrl = 'https://youtube.com';
  </script>
  
  <style>
    .overview {
      text-align: center;
      padding: 20px;
      font-family: Arial, sans-serif;
    }
  
    /* Profile Picture Hover Effect */
    .overview img.profile {
      border-radius: 50%;
      width: 150px;
      height: 150px;
      object-fit: cover;
      margin: 20px 0;
      transition: transform 0.3s ease; /* Smooth transition for the pop-out effect */
    }
  
    /* On hover, scale the profile picture */
    .overview img.profile:hover {
      transform: scale(1.2); /* Slightly increase the size of the profile picture */
    }
  
    .overview h1 {
      font-size: 2rem;
      margin: 10px 0;
    }
  
    .overview .title {
      font-size: 1.2rem;
      margin: 10px 0;
      color: gray;
    }
  
    .overview .links {
      display: flex;
      justify-content: center;
      gap: 20px;
      margin-top: 20px;
    }
  
    .overview .links a {
      color: inherit;
      font-size: 2rem;
      text-decoration: none;
      display: inline-block;
      transition: transform 0.3s ease; /* Smooth transition for the pop-out effect */
    }
  
    /* On hover, scale the icons */
    .overview .links a:hover {
      transform: scale(1.2);
    }
  
    .overview .links img {
      width: 40px;
      height: 40px;
    }
  </style>
  
  <div class="overview">
    <h1>Jerrel Gordon</h1>
    
    <!-- Profile Picture -->
    <img class="profile" src="../assets/jerrel-gordon.png" alt="Jerrel Gordon" />
    
    <p class="title">DevOps Software Engineer</p>
    
    <!-- Links with Icons -->
    <div class="links">
      <a href={githubUrl} target="_blank" title="GitHub">
        <img src="../assets/github-icon.png" alt="GitHub" />
      </a>
      <a href={linkedinUrl} target="_blank" title="LinkedIn">
        <img src="../assets/linkedin-icon.png" alt="LinkedIn" />
      </a>
      <a href={youtubeUrl} target="_blank" title="YouTube">
        <img src="../assets/youtube-icon.png" alt="YouTube" />
      </a>
    </div>
  </div>
  