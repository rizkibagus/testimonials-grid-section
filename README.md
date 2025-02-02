# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)


## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](./design/desktop-preview.jpg)


### Links

- Solution URL: [Add solution URL here](https://github.com/rizkibagus/testimonials-grid-section)
- Live Site URL: [Add live site URL here](https://rizkibagus.github.io/testimonials-grid-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow


### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

```html
  <main class="testimonial-container">
      <article class="testimonial daniel">
        <div class="testimonial-header">
          <img src="./images/image-daniel.jpg" alt="daniel" />
          <div class="testimonial-header-title">
            <h2>Daniel Clifford</h2>
            <p>Verified Graduate</p>
          </div>
        </div>
        <h3>
          I received a job offer mid-course, and the subjects I learned were
          current, if not more so, in the company I joined. I honestly feel I
          got every penny’s worth.
        </h3>
        <p>
          “ I was an EMT for many years before I joined the bootcamp. I’ve been
          looking to make a transition and have heard some people who had an
          amazing experience here. I signed up for the free intro course and
          found it incredibly fun! I enrolled shortly thereafter. The next 12
          weeks was the best - and most grueling - time of my life. Since
          completing the course, I’ve successfully switched careers, working as
          a Software Engineer at a VR startup. ”
        </p>
      </article>

      <article class="testimonial jonathan">
        <div class="testimonial-header">
          <img src="./images/image-jonathan.jpg" alt="daniel" />
          <div class="testimonial-header-title">
            <h2>Jonathan Walters</h2>
            <p>Verified Graduate</p>
          </div>
        </div>
        <h3>The team was very supportive and kept me motivated</h3>
        <p>
          “ I started as a total newbie with virtually no coding skills. I now
          work as a mobile engineer for a big company. This was one of the best
          investments I’ve made in myself. ”
        </p>
      </article>

      <article class="testimonial kira">
        <div class="testimonial-header">
          <img src="./images/image-kira.jpg" alt="daniel" />
          <div class="testimonial-header-title">
            <h2>Kira Whittle</h2>
            <p>Verified Graduate</p>
          </div>
        </div>
        <h3>Such a life-changing experience. Highly recommended!</h3>
        <p>
          “ Before joining the bootcamp, I’ve never written a line of code. I
          needed some structure from professionals who can help me learn
          programming step by step. I was encouraged to enroll by a former
          student of theirs who can only say wonderful things about the program.
          The entire curriculum and staff did not disappoint. They were very
          hands-on and I never had to wait long for assistance. The agile team
          project, in particular, was outstanding. It took my learning to the
          next level in a way that no tutorial could ever have. In fact, I’ve
          often referred to it during interviews as an example of my developent
          experience. It certainly helped me land a job as a full-stack
          developer after receiving multiple offers. 100% recommend! ”
        </p>
      </article>

      <article class="testimonial jeanette">
        <div class="testimonial-header">
          <img src="./images/image-jeanette.jpg" alt="jeanette" />
          <div class="testimonial-header-title">
            <h2>Jeanette Harmon</h2>
            <p>Verified Graduate</p>
          </div>
        </div>
        <h3>An overall wonderful and rewarding experience</h3>
        <p>
          “ Thank you for the wonderful experience! I now have a job I really
          enjoy, and make a good living while doing something I love. ”
        </p>
      </article>

      <article class="testimonial patrick">
        <div class="testimonial-header">
          <img src="./images/image-patrick.jpg" alt="patrick" />
          <div class="testimonial-header-title">
            <h2>Patrick Abrams</h2>
            <p>Verified Graduate</p>
          </div>
        </div>
        <h3>
          Awesome teaching support from TAs who did the bootcamp themselves.
          Getting guidance from them and learning from their experiences was
          easy.
        </h3>
        <p>
          “ The staff seem genuinely concerned about my progress which I find
          really refreshing. The program gave me the confidence necessary to be
          able to go out in the world and present myself as a capable junior
          developer. The standard is above the rest. You will get the personal
          touch from the team. ”
        </p>
      </article>
    </main>
```
```css
 /* Reset basic */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

 body {
    font-family: "Barlow Semi Condensed", serif;
    background-color: var(--light-grayish-blue);
    display: flex;
    padding: 1.5rem 2rem;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
  }

  /* Main container */
  .testimonial-container {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1.5rem;
    max-width: 1100px;
   
  }

  .daniel {
    order: 1;
  }
  .jonathan {
    order: 2;
  }
  .jeanette {
    order: 3;
  }
  .kira {
    order: 5;
  }
  .patrick {
    order: 4;
  }

  .testimonial {
    background: white;
    padding: 1.5rem 1.8rem;
    border-radius: 10px;
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
  }

  .testimonial-header {
    display: flex;
    align-items: center;
    gap: 1rem;
    margin-bottom: 1rem;
  }

    .testimonial-header img {
        width: 40px;
        height: 40px;
        border: 2px solid var(--light-gray);
        border-radius: 50%;
        object-fit: cover;
    }
  
  .testimonial-header-title{
    padding-top: 1.2rem;
    color: var(--white);
  }

    .testimonial-header-title h2 {
        font-size: 0.9rem;
        font-weight: 600;
        margin-bottom: 0.2rem;
    }

    .testimonial-header-title p {
        font-size: 0.7rem;
        font-weight: 500;
        color: var(--light-gray);
    }

    .testimonial-container h3 {
        font-size: 1.2rem;
        font-weight: 600;
        margin-bottom: 1.2rem;
    }

    .testimonial-container p {
        font-size: 0.9rem;
        line-height: 1.3rem;
        font-weight: 500;
        color: var(--light-gray);
        margin-bottom: 1rem;
    }

    article.daniel {
        background: var(--moderate-violet);
        color: var(--white);
        background-image: url(../images/bg-pattern-quotation.svg);
        background-repeat: no-repeat;
        background-position: right 100px top 40px;
        background-size: auto;

        
    }

    article.jonathan {
        background: var(--dark-grayish-blue);
        color: var(--white);
    }

    article.kira .testimonial-header .testimonial-header-title h2,
    article.jeanette .testimonial-header .testimonial-header-title h2
    {
        color: var(--dark-blackish-blue);
    }

    article.kira .testimonial-header .testimonial-header-title p,
    article.jeanette .testimonial-header .testimonial-header-title p
    {
        color: var(--light-gray);
    }

    article.kira p, article.jeanette p {
        color: var(--light-gray);
    }

    article.patrick {
        background: var(--dark-blackish-blue);
        color: var(--white);
    }


  /* Grid responsif */
  @media (min-width: 768px) {
    .testimonial-container {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      grid-template-rows: auto;
      gap: 20px;
      grid-template-areas:
        "daniel daniel jonathan kira"
        "jeanette patrick patrick kira";
    }

    .daniel {
      grid-area: daniel;
    }
    .jonathan {
      grid-area: jonathan;
    }
    .kira {
      grid-area: kira;
    }
    .jeanette {
      grid-area: jeanette;
    }
    .patrick {
      grid-area: patrick;
    }
        
  }

```

## Author

- Website - [Rizki Bagus](https://rizkibagus.github.io/portfolio/)
- Frontend Mentor - [@rizkibagus](https://www.frontendmentor.io/profile/rizkibagus)
- Twitter - [@bagusdev_](https://www.twitter.com/bagusdev_)
