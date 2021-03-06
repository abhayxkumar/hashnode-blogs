## Responsive Portfolio for Web Developers

In this article, we will create a beautiful responsive portfolio page. A portfolio is the most important certificate when applying for a job. The very purpose of your web developer portfolio is to showcase your work(experiences), projects, & education. 

This design is a challenge from devchallenges.io, you can also visit  [there](https://devchallenges.io/challenges/5ZnOYsSXM24JWnCsNFlt)  and complete this challenge.

If you are confused by this application or enjoy watching tutorials. I've included a short video for this program below. Please watch this video!

## Video of Responsive Portfolio

<iframe width="1182" height="665" src="https://www.youtube.com/embed/lXaSnyvz9jY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

*For image files, you can find the Github Repository link in the YouTube video description.*


## Source Code

To copy the program's provided codes, you should first create two files, one of which is an HTML file and the other of which is a CSS file. You can copy-paste the provided codes into your files after you've created these two files.

### HTML Code:-


```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta
      name="viewport"
      content="width=device-width, initial-scale=1,
  maximum-scale=5"
    />

    <link rel="icon" href="images/devchallenges.png" />

    <link
      rel="shortcut icon"
      type="image/x-icon"
      href="https://devchallenges.io/"
    />

    <title>Portfolio</title>

    <link rel="stylesheet" href="style.css">

  </head>
  <body>
    <div class="profile__card card">
      <div class="profile__avatar">
        <img src="images/cropped-profile.png" alt="photo of a person smiling">
      </div>
      <div class="profile__info">
        <p>Billy Pearson</p>
        <p>Front-end developer</p>
      </div>
      <div class="profile__contact">
        <div class="contact__email">
          <img src="images/email-black-18dp.svg" alt="email icon">
          <p>billy@example.com</p>
        </div>
        <div class="contact__phone">
          <img src="images/phone-black-18dp.svg" alt="">
          <p>(+603) 546 624 342</p>
        </div>
      </div>
      <div class="profile__description">
        <p>Self-motivated developer, who is willing to learn and create outstanding UI applications.
        </p>
      </div>
    </div>
  
    <!-- Section for skills -->
    <section class="skills">
      <div class="skills__card card">
        <h4>Front End</h4>
        <div class="tech__skill">
          <p>React</p>
          <div class="tech__scale">
            <div class="tech__percent react"></div>
          </div>
        </div>
        <div class="tech__skill">
          <p>Javascript</p>
          <div class="tech__scale">
            <div class="tech__percent javascript"></div>
          </div>
        </div>
        <div class="tech__skill">
          <p>CSS</p>
          <div class="tech__scale">
            <div class="tech__percent css"></div>
          </div>
        </div>
        <div class="tech__skill">
          <p>Vue</p>
          <div class="tech__scale">
            <div class="tech__percent vue"></div>
          </div>
        </div>
        <div class="tech__skill">
          <p>Redux</p>
          <div class="tech__scale">
            <div class="tech__percent redux"></div>
          </div>
        </div>
        <div class="tech__skill">
          <p>React Native</p>
          <div class="tech__scale">
            <div class="tech__percent reactnative"></div>
          </div>
        </div>
      </div>
  
      <div class="skills__card tech__skills card">
        <h4>Design</h4>
        <div class="tech__skill">
          <p>Figma</p>
          <div class="tech__scale">
            <div class="tech__percent figma"></div>
          </div>
        </div>
        <div class="tech__skill">
          <p>Photoshop</p>
          <div class="tech__scale">
            <div class="tech__percent photoshop"></div>
          </div>
        </div>
      </div>
    </section>
  
    <!-- Section for projects -->
    <section class="projects">
      <div class="project__count card">
        <h5>Projects (3)</h5>
      </div>
  
      <!-- First project -->
      <div class="project__card card">
        <div class="project__cover">
          <img src="images/recipe-project-sm.png" alt="">
        </div>
        <div class="project__about">
          <div class="project__tag">
            <p class="tag">#HTML</p>
            <p class="tag">#CSS</p>
            <p class="tag">#responsive</p>
          </div>
          <h2 class="project__title">Recipe Blog</h2>
          <p class="project__details">In this project, I work with HTML and CSS to create a responsive
            page . The design is from devchallenge.io. Donec aliquam est dui, vel vestibulum diam
            sollicitudin id. Quisque feugiat malesuada molestie. </p>
          <div class="buttons">
            <button class="btn--primary"><a
                href="#">Demo</a></button>
            <button><a
                href="#">Code</a></button>
          </div>
        </div>
      </div>
  
      <!-- Second project -->
      <div class="project__card card">
        <div class="project__cover">
          <img src="images/gallery-project-sm.png" alt="">
        </div>
        <div class="project__about">
          <div class="project__tag">
            <p class="tag">#HTML</p>
            <p class="tag">#CSS</p>
            <p class="tag">#responsive</p>
          </div>
          <h2 class="project__title">My Gallery</h2>
          <p class="project__details">In this project, I work with HTML and CSS to create a responsive
            page . The design is from devchallenge.io. Donec aliquam est dui, vel vestibulum diam
            sollicitudin id. Quisque feugiat malesuada molestie. </p>
          <div class="buttons">
            <button class="btn--primary"><a
                href="#">Demo</a></button>
            <button><a
                href="#">Code</a></button>
          </div>
        </div>
      </div>
  
      <!-- Third project -->
      <div class="project__card card">
        <div class="project__cover">
          <img src="images/checkout-project-sm.png" alt="">
        </div>
        <div class="project__about">
          <div class="project__tag">
            <p class="tag">#HTML</p>
            <p class="tag">#CSS</p>
            <p class="tag">#responsive</p>
          </div>
          <h2 class="project__title">Checkout</h2>
          <p class="project__details">In this project, I work with HTML and CSS to create a responsive
            page . The design is from devchallenge.io. Donec aliquam est dui, vel vestibulum diam
            sollicitudin id. Quisque feugiat malesuada molestie. </p>
          <div class="buttons">
            <button class="btn--primary"><a
                href="#">Demo</a></button>
            <button><a
                href="#">Code</a></button>
          </div>
        </div>
      </div>
    </section>
  
    <!-- Blog section -->
    <section class="blog">
      <div class="blog__count card">
        <h5>Blogs (1)</h5>
      </div>
  
      <div class="blog__card card card--blog">
        <p class="blog__tag">Blog</p>
        <div class="blog__cover">
          <div class="blog__title">
            <h3>How to organize your CSS</h3>
          </div>
          <div class="blog__image">
            <img src="images/blog-image-sm.jpg" alt="">
          </div>
        </div>
        <div class="blog__details">
          <p>In this article I tell the story about Proin eu justo sit amet lacus bibendum tincidunt.
            Vivamus non volutpat nisl, a luctus mi.</p>
          <p>Donec aliquam est dui, vel vestibulum diam sollicitudin id. Quisque feugiat malesuada
            molestie.</p>
        </div>
        <p class="blog__platform">dev.to</p>
      </div>
    </section>
  
    <!-- Experience section -->
    <section class="experience">
      <div class="experience__card card">
        <h3>Experience</h3>
        <div class="experience__item">
          <div class="experience__logo">
            <img src="images/adidas-logo.svg" alt="">
          </div>
          <div class="experience__about">
            <p class="experience__date">Feb 2017 - Current</p>
            <p class="experience__position">Front-end developer</p>
            <p class="experience__role">Donec aliquam est dui, vel vestibulum diam sollicitudin id.
              Quisque feugiat malesuada molestie.</p>
          </div>
        </div>
        <div class="experience__item">
          <div class="experience__logo">
            <img src="images/H&M-logo.png" alt="">
          </div>
          <div class="experience__about">
            <p class="experience__date">Aug 2016 - Feb 2018</p>
            <p class="experience__position">Full-stack developer</p>
            <p class="experience__role">Donec aliquam est dui, vel vestibulum diam sollicitudin id.
              Quisque feugiat malesuada molestie.</p>
          </div>
        </div>
        <div class="experience__item">
          <div class="experience__logo">
            <img src="images/nivea-logo.png" alt="">
          </div>
          <div class="experience__about">
            <p class="experience__date">Jun 2015 - Aug 2016</p>
            <p class="experience__position">Junior front-end developer</p>
            <p class="experience__role">Donec aliquam est dui, vel vestibulum diam sollicitudin id.
              Quisque feugiat malesuada molestie.</p>
          </div>
        </div>
      </div>
    </section>
  
    <!-- Hobby section -->
    <section class="hobby">
      <div class="hobby__card card">
        <h3>Hobbies</h3>
        <div class="hobby__item">
          <div class="hobby__image">
            <img src="images/gaming.jpg" alt="">
          </div>
          <div class="hobby__about">
            <p class="hobby__title">Gaming</p>
            <p class="hobby__about">Quisque feugiat malesuada molestie.</p>
          </div>
        </div>
        <div class="hobby__item">
          <div class="hobby__image">
            <img src="images/cooking.jpg" alt="">
          </div>
          <div class="hobby__about">
            <p class="hobby__title">Cooking</p>
            <p class="hobby__about">Quisque feugiat malesuada molestie.</p>
          </div>
        </div>
        <div class="hobby__item">
          <div class="hobby__image">
            <img src="images/biking.jpg" alt="">
          </div>
          <div class="hobby__about">
            <p class="hobby__title">Biking</p>
            <p class="hobby__about">Quisque feugiat malesuada molestie.</p>
          </div>
        </div>
      </div>
    </section>
  
    <footer>
      <a href="https://github.com/abhayxkumar">Abhay Kumar</a><a
        href="https://devchallenges.io/challenges"> @DevChallenges.io</a>
    </footer>
  </body>
</html>

``` 

### CSS Code:-


```
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
  
  :root {
    /* Colors */
    --white001: #ffffff;
    --gray001: #4f4f4f;
    --gray002: #828282;
    --gray003: #c4c4c4;
    --gray004: #f2f2f2;
    --gray005: #e0e0e0;
    --gray006: #a9a9a9;
    --primary: #5c94e1;
    --primary-hover: #cedef6;
    --progress: rgba(47, 128, 237, 70%);
  
    /* Border radius */
    --border-radius: 12px;
    /* margin*/
    --margin-small: 0.5rem;
    --margin-medium: 1rem;
    --margin-large: 1.5rem;
  }
  
  body {
    font-family: "Montserrat", sans-serif;
    background-color: var(--gray004);
    margin: 1rem;
    color: var(--gray001);
  }
  
  img {
    display: block;
  }
  
  p {
    font-size: 0.825rem;
    line-height: 18.5px;
  }
  
  .card {
    background-color: var(--white001);
    border-radius: var(--border-radius);
    padding: 1rem;
    box-shadow: 0px 4px 32px rgba(0, 0, 0, 0.12);
    margin-bottom: var(--margin-medium);
  }
  
  /* Profile card styles */
  .profile__card {
    margin-bottom: var(--margin-medium);
    display: flex;
    flex-direction: column;
  }
  
  .profile__avatar {
    border-radius: var(--border-radius);
    overflow: hidden;
    width: 100%;
    max-width: 25rem;
    margin-bottom: var(--margin-medium);
  }
  
  .profile__avatar img {
    width: 100%;
    object-fit: cover;
  }
  
  .profile__info {
    margin-bottom: var(--margin-medium);
  }
  .profile__info p:first-child {
    font-weight: 600;
    font-size: 1.25rem;
  }
  
  .profile__info p:last-child,
  .profile__description {
    color: var(--gray002);
    font-size: 0.875rem;
    width: 80%;
  }
  
  .profile__contact {
    margin-bottom: var(--margin-medium);
  }
  
  .contact__email,
  .contact__phone {
    transition: 0.2s ease-out color;
    cursor: pointer;
    display: flex;
    align-items: center;
    margin-bottom: var(--margin-small);
  }
  .contact__email img,
  .contact__phone img {
    margin-right: var(--margin-small);
  }
  
  /* Skills cards styles */
  .skills {
    margin-bottom: var(--margin-medium);
  }
  .skills__card h4 {
    text-transform: uppercase;
    margin-bottom: var(--margin-medium);
  }
  
  .tech__skill {
    display: flex;
    align-items: center;
    margin-bottom: var(--margin-medium);
  }
  
  .tech__scale {
    margin-left: auto;
    border-radius: 7px;
    width: 60%;
    height: 0.5rem;
    background-color: var(--gray003);
  }
  
  .tech__percent {
    height: 0.5rem;
    border-radius: 5px;
    background-color: var(--progress);
  }
  
  /* Different levels for progress bar */
  .react {
    width: 60%;
  }
  
  .javascript {
    width: 83%;
  }
  
  .css {
    width: 95%;
  }
  
  .vue {
    width: 56%;
  }
  
  .redux {
    width: 75%;
  }
  
  .reactnative {
    width: 93%;
  }
  
  .figma {
    width: 60%;
  }
  
  .photoshop {
    width: 83%;
  }
  
  /* Styles for project cards */
  
  .project__count,
  .blog__count {
    margin-bottom: var(--margin-medium);
  }
  .project__card {
    margin-bottom: var(--margin-large);
  }
  
  .project__card p {
    color: var(--gray002);
  }
  
  .project__cover {
    width: 100%;
    overflow: hidden;
    height: 15rem;
    margin-bottom: var(--margin-medium);
    border-radius: var(--border-radius);
  }
  
  .project__cover img {
    width: 100%;
    height: 100%;
  }
  
  .project__tag {
    display: flex;
  }
  
  .project__tag > p {
    margin-right: var(--margin-small);
    margin-bottom: var(--margin-medium);
  }
  
  .project__title {
    margin-bottom: var(--margin-medium);
  }
  
  .project__details {
    margin-bottom: var(--margin-large);
  }
  
  button {
    border: none;
    margin-bottom: var(--margin-small);
    margin-right: var(--margin-small);
  }
  
  button a {
    text-decoration: none;
    color: var(--progress);
    border-radius: var(--border-radius);
    border: 1px solid var(--progress);
    background-color: var(--white001);
    padding: 0.5rem 2rem;
    transition: 0.2s ease-out all;
  }
  
  .btn--primary a {
    background-color: var(--progress);
    color: var(--white001);
    border: none;
  }
  
  /* Styles for blog section */
  .blog__tag,
  .blog__platform {
    color: var(--gray005);
    font-size: 0.825rem;
    margin-bottom: var(--margin-medium);
  }
  
  .blog__cover {
    display: flex;
    overflow: hidden;
    margin-bottom: var(--margin-medium);
  }
  
  .blog__title {
    width: 50%;
  }
  
  .blog__title h2 {
    font-weight: 500;
  }
  
  .blog__image {
    width: 60%;
    transform: translateX(5%);
    height: 11rem;
    overflow: hidden;
  }
  
  .blog__image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  
  .blog__details {
    margin-bottom: var(--margin-large);
  }
  
  .blog__details p {
    color: var(--gray002);
    margin-bottom: var(--margin-medium);
    padding-right: 1rem;
  }
  
  .card--blog {
    padding-right: 0;
  }
  
  .blog__platform {
    color: var(--progress);
    margin-bottom: 0;
  }
  
  /* Shared styles */
  section {
    margin-bottom: var(--margin-medium);
  }
  
  .experience__card h3,
  .hobby__card h3 {
    margin-bottom: var(--margin-medium);
  }
  
  .experience__position,
  .hobby__title {
    font-weight: 600;
    font-size: 15px;
    margin-bottom: var(--margin-small);
  }
  
  /* Experience section styles */
  
  .experience__item {
    display: flex;
    margin-bottom: var(--margin-large);
  }
  
  .experience__logo {
    width: 30%;
    margin-right: var(--margin-medium);
    overflow: hidden;
  }
  
  .experience__logo img {
    width: 100%;
  }
  .experience__date {
    margin-bottom: var(--margin-small);
  }
  
  .experience__date,
  .experience__role {
    color: var(--gray002);
  }
  
  /* Styles for hobby section */
  .hobby,
  .hobby__item {
    margin-bottom: var(--margin-large);
  }
  
  .hobby__image {
    width: 100%;
    height: 10rem;
    overflow: hidden;
    border-radius: var(--border-radius);
    margin-bottom: var(--margin-medium);
  }
  
  .hobby__image img {
    width: 100%;
  }
  
  /* Footer styles */
  footer {
    width: 100%;
    text-align: center;
  }
  
  footer a {
    border-top: 1px solid var(--gray006);
    padding-top: 0.5rem;
    font-weight: 600;
    text-decoration: none;
    font-size: 0.75rem;
    color: var(--gray006);
    transition: 0.2s ease-out color;
  }
  
  /* Hover states */
  @media (hover: hover) {
    button a:hover {
      color: var(--primary-hover);
      border-color: var(--primary-hover);
    }
  
    .btn--primary a:hover {
      background-color: var(--primary-hover);
      color: var(--primary);
    }
  
    .contact__email:hover,
    .contact__phone:hover,
    footer a:hover {
      color: var(--primary);
    }
  }
  
  /* Screen sizes */
  @media screen and (min-width: 720px) {
    body {
      display: grid;
      grid-template-rows: 17rem 9rem 3rem 1fr;
      grid-template-columns: repeat(6, 1fr);
      gap: 1rem;
    }
  
    .profile__card {
      grid-column: 1 / span 3;
      grid-row: span 3;
    }
  
    .skills {
      grid-row: 1 / 2;
      grid-column: 4 / span 3;
    }
  
    .skills__tech {
      grid-row: 2;
      grid-column: 4 / span 3;
    }
  
    .projects {
      grid-row: 3;
      grid-column: 4 / span 3;
    }
    .project__card {
      height: auto;
    }
  
    .experience {
      grid-column: span 3;
      grid-row: 4;
    }
  
    .experience__logo {
      width: 40%;
    }
  
    .hobby {
      grid-column: span 3;
      grid-row: 5 / span 3;
    }
  
    .blog {
      grid-column: span 3;
      grid-row: 8;
      transform: translateY(-2rem);
    }
  
    footer {
      grid-row: 10;
      grid-column: span 6;
    }
  }
  
  @media screen and (min-width: 1100px) {
    body {
      min-height: 100vh;
      display: grid;
      /* grid-template-rows: 17rem 15rem 15rem auto 1fr 1fr; */
      grid-template-columns: repeat(12, 1fr);
      padding: 1rem;
      max-width: 1250px;
      margin: 0 auto;
    }
  
    .profile__card {
      grid-column: 1 / span 4;
      height: 35rem;
    }
  
    .skills {
      grid-column: 5 / span 9;
      display: flex;
    }
  
    .skills__card {
      width: 50%;
      height: 100%;
    }
  
    .tech__skills {
      margin-left: var(--margin-medium);
      height: 50%;
    }
  
    .projects {
      grid-row: 2;
      grid-column: 5 / span 8;
    }
  
    .project__card {
      display: flex;
      margin-bottom: var(--margin-large);
    }
  
    .project__cover {
      width: 50%;
      height: 15rem;
      overflow: hidden;
    }
  
    .project__cover img {
      height: 100%;
      width: 100%;
    }
  
    .project__about {
      margin-left: auto;
      width: 47%;
      height: 15rem;
      display: flex;
      flex-direction: column;
    }
  
    .project__details {
      flex: 1;
    }
  
    .blog {
      transform: translateY(-3rem);
      grid-row: 7;
      grid-column: 5 / span 8;
    }
  
    .experience {
      transform: translateY(4rem);
      grid-column: 1 / span 4;
    }
  
    .blog__cover,
    .blog__image {
      height: 15rem;
    }
    .hobby {
      transform: translateY(2rem);
      grid-column: 1 / span 4;
    }
  
    footer {
      grid-column: 5 / span 4;
      border-top: 1px solid var(--gray006);
    }
    footer a {
      border-top: none;
    }
  }
``` 

