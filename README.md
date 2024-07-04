# css-advanced-project

Create a simplified clone of Dribbble landing page.


## index.html

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dribbble Clone</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <nav>
      <div class="logo">Dribbble</div>
      <ul class="nav-links">
        <li><a href="#">Shots</a></li>
        <li><a href="#">Designers</a></li>
        <li><a href="#">Teams</a></li>
        <li><a href="#">Community</a></li>
        <li><a href="#">Jobs</a></li>
      </ul>
      <div class="auth-search-container">
        <div class="auth-buttons">
          <a href="#" class="btn login">Sign In</a>
          <a href="#" class="btn signup">Sign Up</a>
        </div>
        <div class="search-bar">
          <input type="text" placeholder="Search">
        </div>
      </div>
    </nav>
  </header>

  <section class="featured-message">
    <p>What are you working on? Dribbble is show and tell for designers.</p>
    <a href="#" class="btn learn-more">Learn more</a>
    <a href="#" class="btn sign-up">Sign up</a>
  </section>

  <section class="projects">
    <div class="projects-header">
      <div class="filters">
        <span>Popular &#9662;</span>
        <span>Shots &#9662;</span>
        <span>Now &#9662;</span>
      </div>
    </div>
    <div class="project-grid">
      <div class="project-card">
        <img src="C:/Users/user/Downloads/s1.jpg" alt="Project 1">
      </div>
      <div class="project-card">
        <img src="C:/Users/user/Downloads/s2.jpg" alt="Project 2">
      </div>
      <div class="project-card">
        <img src="C:/Users/user/Downloads/s3.jpg" alt="Project 3">
      </div>
      <div class="project-card">
        <img src="C:/Users/user/Downloads/s4.jpg" alt="Project 4">
      </div>
      <div class="project-card">
        <img src="C:/Users/user/Downloads/s5.jpg" alt="Project 5">
      </div>
      <div class="project-card">
        <img src="C:/Users/user/Downloads/s6.jpg" alt="Project 6">
      </div>
      <div class="project-card">
        <img src="C:/Users/user/Downloads/s7.jpg" alt="Project 7">
      </div>
      <div class="project-card">
        <img src="C:/Users/user/Downloads/s8.jpg" alt="Project 8">
      </div>
      <div class="project-card">
        <img src="C:/Users/user/Downloads/s9.jpg" alt="Project 9">
      </div>
      <div class="project-card">
        <img src="C:/Users/user/Downloads/s10.jpg" alt="Project 10">
      </div>
      <div class="project-card">
        <img src="C:/Users/user/Downloads/s11.jpg" alt="Project 11">
      </div>
      <div class="project-card">
        <img src="C:/Users/user/Downloads/s12.jpg" alt="Project 12">
      </div>
      <div class="project-card">
        <img src="C:/Users/user/Downloads/s13.jpg" alt="Project 13">
      </div>
      <div class="project-card">
        <img src="C:/Users/user/Downloads/s14.jpg" alt="Project 14">
      </div>
      <div class="project-card">
        <img src="C:/Users/user/Downloads/s15.jpg" alt="Project 15">
      </div>
      <div class="project-card">
        <img src="C:/Users/user/Downloads/s16.jpg" alt="Project 16">
      </div>

    </div>
  </section>

  <footer>
    <p>© 2024 Dribbble. All rights reserved.</p>
  </footer>
</body>
</html>
```


## styles.css

```
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
}

header {
  background: #333;
  color: #fff;
  padding: 10px 20px;
  position: sticky;
  top: 0;
  z-index: 1000;
}

nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
  color: #ea4c89;
}

.nav-links {
  list-style: none;
  display: flex;
  margin-left: 20px;
}

.nav-links li {
  margin-left: 20px;
}

.nav-links a {
  text-decoration: none;
  color: #fff;
  font-weight: 500;
}

.auth-search-container {
  display: flex;
  align-items: center;
}

.auth-buttons .btn {
  padding: 10px 20px;
  border-radius: 5px;
  margin-left: 10px;
  text-decoration: none;
  color: #fff;
}

.auth-buttons .login {
  background: #444;
}

.auth-buttons .signup {
  background: #ea4c89;
}

.search-bar {
  margin-left: 10px;
}

.search-bar input {
  padding: 10px;
  border-radius: 5px;
  border: 1px solid #ccc;
}

.featured-message {
  background: #000;
  color: #fff;
  padding: 20px;
  text-align: center;
}

.featured-message p {
  margin-bottom: 10px;
  font-size: 1.2rem;
}

.featured-message .btn {
  padding: 10px 20px;
  border-radius: 5px;
  text-decoration: none;
  margin: 0 10px;
}

.learn-more {
  background: #444;
  color: #fff;
}

.sign-up {
  background: #ea4c89;
  color: #fff;
}

.projects {
  padding: 40px 20px;
}

.projects-header {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 20px;
}

.projects-header h2 {
  font-size: 1.5rem;
  margin-right: auto;
}

.filters {
  display: flex;
  gap: 10px;
}

.filters span {
  background: #e1e1e1;
  padding: 5px 10px;
  border-radius: 5px;
}

.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
}

.project-card {
  background: #fff;
  border-radius: 10px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  padding: 20px;
  text-align: center;
}

.project-card img {
  width: 100%;
  border-radius: 10px;
  margin-bottom: 10px;
}

footer {
  background: #333;
  color: #fff;
  text-align: center;
  padding: 20px 0;
}
```



## OUTPUT


![output](https://github.com/SmritiManikand/css-advanced-project/assets/113674204/a1a14470-10f1-412d-8928-72702375901d)

