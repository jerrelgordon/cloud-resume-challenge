<script>
    import { onMount } from 'svelte';
  
    let visitorCount = 'Loading...'; // Default state is just a stuck loading text
  
    // Fetch visitor count from the API
    onMount(async () => {
      try {
        const response = await fetch('https://67xj8wdsrj.execute-api.us-east-1.amazonaws.com/prod/count');
        const data = await response.json();
        // Parse the visitor count based on the response structure
        const count = data.body ? JSON.parse(data.body).visitor_count : data.visitor_count;
        visitorCount = count;
      } catch (error) {
        console.error('Error fetching visitor count:', error);
        visitorCount = 'Error loading visitor count';
      }
    });
  </script>
  
  <p>{`${visitorCount} site views`}</p>
  
  <style>
    p {
      font-size: 1.2rem;
      font-weight: bold;
      color: #fff;
    }
  </style>
  