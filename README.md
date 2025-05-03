<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Our Pricing Plans</title>
  <style>
    body {
      /* Use a standard, professional font stack */
      font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
      background-color: #f8f9fa; /* Lighter, standard gray */
      color: #343a40; /* Darker gray for main text */
      text-align: center;
      padding: 40px 20px; /* Increased top/bottom padding */
      margin: 0;
      line-height: 1.6; /* Improved readability */
    }

    h1 {
      font-size: 2.5em; /* Slightly adjusted size */
      color: #343a40; /* Standard dark heading color */
      margin-bottom: 40px;
    }

    .pricing-container {
      display: grid;
      /* Maintain the responsive grid layout */
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); /* More flexible grid */
      gap: 30px; /* Slightly increased gap */
      max-width: 1100px; /* Set a max-width for larger screens */
      margin: 40px auto 0; /* Center the container */
      padding: 0 20px; /* Add horizontal padding */
    }

    /* No need for media query if using auto-fit minmax correctly */
    /* @media (max-width: 768px) { ... } */

    .pricing-card {
      background: #ffffff; /* Pure white background */
      border: 1px solid #dee2e6; /* Subtler border */
      border-radius: 8px; /* Slightly smaller radius */
      padding: 30px; /* Increased padding */
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08); /* Softer shadow */
      display: flex; /* Use flexbox for better internal alignment */
      flex-direction: column;
      text-align: left; /* Align text left within cards */
    }

    .pricing-card h2 {
      font-size: 1.8em;
      color: #343a40;
      margin-bottom: 10px;
      text-align: center; /* Center plan title */
    }

    .pricing-card .plan-description { /* Added class for clarity */
      font-size: 1em;
      color: #6c757d; /* Standard secondary text color */
      margin-bottom: 20px;
      min-height: 40px; /* Ensure consistent height */
       text-align: center; /* Center description */
    }

    .pricing-card .price {
      font-size: 2.2em;
      font-weight: 600; /* Bolder price */
      color: #007bff; /* Professional blue color */
      margin: 20px 0;
      text-align: center; /* Center price */
    }
     .pricing-card .price span { /* Style for per month/etc. */
       font-size: 0.6em;
       font-weight: 400;
       color: #6c757d;
     }

    .feature-list {
      list-style: none; /* Remove default bullets */
      padding: 0;
      margin: 20px 0 30px; /* Adjusted margins */
      font-size: 0.95em;
      color: #495057; /* Slightly darker feature text */
      flex-grow: 1; /* Make feature list fill available space */
    }

    .feature-list li {
      margin-bottom: 12px;
      padding-left: 25px; /* Space for icon */
      position: relative;
    }

     /* Add checkmark icons for features */
    .feature-list li::before {
        content: '✔'; /* Simple checkmark */
        color: #28a745; /* Green color for checkmark */
        position: absolute;
        left: 0;
        top: 1px;
        font-weight: bold;
    }

    .pricing-card button {
      background: #007bff; /* Professional blue */
      color: #ffffff;
      border: none;
      padding: 12px 20px; /* Slightly larger padding */
      border-radius: 5px;
      font-size: 1.1em; /* Slightly larger font */
      font-weight: 500;
      cursor: pointer;
      width: 100%;
      margin-top: auto; /* Push button to bottom */
      transition: background-color 0.2s ease-in-out; /* Smooth hover transition */
    }

    .pricing-card button:hover {
      background: #0056b3; /* Darker blue on hover */
    }

    /* Style for the most popular plan (optional) */
    .pricing-card.popular {
        border-color: #007bff;
        box-shadow: 0 6px 16px rgba(0, 123, 255, 0.2);
    }
     .pricing-card.popular h2 {
         color: #007bff;
     }

  </style>
</head>
<body>

  <h1>Our Pricing Plans</h1>

  <div class="pricing-container">
    <div class="pricing-card">
      <h2>Basic</h2>
      <p class="plan-description">Ideal for trying out the platform.</p>
      <div class="price">$0 <span>/ month</span></div>
      <ul class="feature-list">
        <li>Core Features Access</li>
        <li>1 Project Allowed</li>
        <li>Community Support</li>
        <li>Basic Analytics</li>
        </ul>
      <button>Get Started</button>
    </div>

    <div class="pricing-card popular"> <h2>Pro (Lifetime)</h2>
      <p class="plan-description">One-time purchase for full access to current features.</p>
      <div class="price">$6 <span>one-time</span></div>
      <ul class="feature-list">
        <li>Supporting the developer</li>
        <li>All Core Features</li>
        <li>Up to 10 Projects</li>
        <li>Email Support</li>
        <li>Advanced Analytics</li>
        </ul>
       <button>Purchase Now</button>
    </div>

    <div class="pricing-card">
      <h2>Business</h2>
      <p class="plan-description">Best for ongoing business needs and priority support.</p>
      <div class="price">$1 <span>/ Month</span></div>
      <ul class="feature-list">
        <li>Continuously supporting developers</li>
        <li>one license per user</li>
		<li>All Pro Features</li>
        <li>Unlimited Projects</li>
        <li>Priority Email</li>
        <li>Chat Support</li>
        <li>Advanced Analytics</li>
        </ul>
      <button>Subscribe</button>
    </div>
  </div>

  </body>
</html>
