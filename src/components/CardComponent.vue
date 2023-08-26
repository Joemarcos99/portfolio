<template>
    <div class="card">
      <h2>{{ title }}</h2>
      <div class="description">
        <p> Computer Science Student @ University of Michigan</p>
      </div>
      <div class="links">
        <a :href="linkedin" target="_blank">
          <img src="/linkedin-logo.png" alt="LinkedIn Profile" class="icon"/>
        </a>
        <a :href="'mailto:' + email">
          <img src="/email-logo.jpg" alt="Email Link" class="icon"/>
        </a>
        <a :href="github" target="_blank">
          <img src="/github-logo.jpg" alt="Github Profile" class="icon"/>
        </a>
      </div>
      <a :href=resumePath download="Joseph-Marcotte-Resume.pdf" class="download-button">Download Resume</a>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      title: String,
      linkedin: String,
      email: String,
      github: String,
      resumePath: String,
    },
  };
  </script>
  
  <style scoped>

  a:hover {
    opacity: .7;
  }

  h2 {
    color: rgb(0, 0, 0);
    text-align: center;
    text-shadow: 2px 0 #fff, -2px 0 #fff, 0 2px #fff, 0 -2px #fff,
               1px 1px #fff, -1px -1px #fff, 1px -1px #fff, -1px 1px #fff;
  }

  p {
    color: black;
    margin: .2rem;
  }
  .card {
    border: 2px solid #ccc;
    padding: 20px;
    margin: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    background-color: #442f61;
  }

  .icon {
    width: 40px;
    height: 40px;
    margin: 10px;
  }
  
  .links {
    margin-top: 10px;
    margin-bottom: 10px;
    display: flex;
    justify-content: center;
  }

  .description {
    border-radius: 8px;
    background-color: white;
    padding-left: 1rem;
    padding-right: 1rem;
  }
  
  .links a {
    margin-right: 10px;
  }

  .download-button {
    display: flex;
    justify-content: center;
    margin-top: 10px;
    padding: 8px 16px;
    background-color: #D86018;
    color: #fff;
    text-decoration: none;
    border-radius: 4px;
  }
  </style>