<template>
  <main>
    <a name="home"></a>
    <section id="landing">
      <img
        class="landing"
        src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/landing.jpg"
        alt=""
      />
      <div>
        <h1>I am Seth Tobias.</h1>
        <div class="line"></div>
        <h2>An aspiring developer.</h2>
      </div>
    </section>

    <section id="about">
      <a name="about"></a>
      <div class="container about">
        <div class="heading">
          <h2>About</h2>
          <div class="line"></div>
        </div>
        <div class="content about">
          <p>
            I am a 19-year-old with a passion for coding and strong
            communication skills in English and Afrikaans. After completing a
            six-month program at Life Choices Academy, my dedication to coding
            intensified, leading me to pursue an internship at LC Studios within
            the ICT industry. I am driven by my love for Hockey, where I have
            learnt resilience, teamwork, and the joy of sports. Additionally, I
            indulge in hobbies like watching movies, reading Manga and Manhua,
            creating meaningful music playlists and gaming, which sparked my
            interest in coding and web development.
          </p>
          <div class="about-img">
            <img
              class="about img"
              src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/LC-Headshot2.jpg"
              alt=""
            />
          </div>
        </div>
      </div>
    </section>

    <section id="projects">
      <a name="projects"></a>
      <CertModal
        :isVisible="isModalVisible"
        :title="modalTitle"
        :msg="modalMsg"
        :git="modalGit"
        :link="modalLink"
        @close="closeModal"
      ></CertModal>
      <div class="container projects">
        <div class="heading">
          <h2>Projects</h2>
          <div class="line"></div>
        </div>
        <div class="projects">
          <div class="project one">
            <img
              @click="
                openModal(
                  'Time Converter',
                  'This was one of the very first JavaScript projects I was assigned. It was a simple time converter to go from minutes to seconds. Overtime however I improved the functionality and overall styling of the project to the current point it is at now. It taught me the basics of DOM manipulation and the basics of how operators in JavaScript work.',
                  'https://github.com/SethTobias/TimeConverter',
                  'https://jovial-biscuit-82d853.netlify.app'
                )
              "
              src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/time-converter.png"
              alt=""
            />
          </div>
          <div class="project two">
            <img
              @click="
                openModal(
                  'Momentum Motors',
                  'This was the very first project I completed while working with another developer. The project highlighted the importance of effective communication. We were also tasked for the first time to work with a database through the use of MySQL and the use of Node.js in order to effectively communicate with the database.',
                  'https://github.com/SethTobias/Node_Eomp',
                  'https://node-js-562d4.web.app/'
                )
              "
              src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/momentum-motors.png"
              alt=""
            />
          </div>
          <div class="project three">
            <img
              @click="
                openModal(
                  'Literaty Connect',
                  'Through this project I completed my first Full-stack application/website. I completed a social media website where I implemented the basic functionality as seen in many other social media platforms.',
                  'https://github.com/SethTobias/Literary_Connect',
                  'https://literary-connect.web.app/'
                )
              "
              src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/literary-connect.png"
              alt=""
            />
          </div>
        </div>
      </div>
    </section>

    <section id="experience">
      <a name="expertise"></a>
      <a name="experience"></a>
      <div class="container experience">
        <div class="heading">
          <h2>Experience</h2>
          <div class="line"></div>
        </div>
        <div class="item one">
          <div class="time-text">
            <h3>LC Studio</h3>
            <p>
              After finishing a six-month Full-stack Web Development bootcamp, I
              gained expertise in both front-end and back-end development. Now,
              as an Intern at LC Studios, I'm applying these skills
              professionally, refining them further and contributing to
              impactful projects under mentorship.
            </p>
          </div>
          <div class="time-line">
            <p>2024/04/01</p>
            <i class="fa-solid fa-code-fork"></i>
            <div></div>
          </div>
          <div class="time-img">
            <img
              src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/lc_studio.png"
              alt=""
            />
          </div>
        </div>
      </div>
    </section>

    <section id="education">
      <a name="education"></a>
      <div class="container education">
        <div class="heading">
          <h2>Education</h2>
          <div class="line"></div>
        </div>
        <div class="item one">
          <div class="time-text">
            <h3>Life Choices Academy</h3>
            <p>
              During an intensive six-month Full-Stack Web Development Course at
              Life Choices Academy, I gained proficiency in foundational tools
              like Figma, HTML, CSS, and JavaScript in the first three months.
              The course then advanced to cover SQL, Vue.js, and Node.js,
              providing me with a comprehensive skill set and adaptability for
              industry demands as a Web Developer.
            </p>
          </div>
          <div class="time-line">
            <p>2024/03/29</p>
            <i class="fa-solid fa-laptop-code"></i>
            <div></div>
          </div>
          <div class="time-img">
            <img
              src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/life_choices_academy_logo.png"
              alt=""
            />
          </div>
        </div>

        <div class="item two">
          <div class="time-text">
            <h3>Table View Highschool</h3>
            <p>
              I attended Table View High School for 5 years, completing my NSC
              qualification with a Bachelor's Pass. My subjects included English
              HL, Afrikaans FAL, Mathematics, Life Orientation, Computer
              Applications Technology, Physical Sciences, and Life Sciences.
              Notably, I achieved distinctions in Computer Applications
              Technology (82%) and Life Sciences (80%).
            </p>
          </div>
          <div class="time-line">
            <p>2024/10/30</p>
            <i class="fa-solid fa-book-bookmark"></i>
            <div></div>
          </div>
          <div class="time-img">
            <img
              src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/tvhs_logo.png"
              alt=""
            />
          </div>
        </div>
      </div>
    </section>

    <section id="r_resources">
      <a name="resources"></a>
      <div class="container resources">
        <div class="heading">
          <h2>Related Resources</h2>
          <div class="line"></div>
        </div>
        <div class="downloads">
          <div class="ditem 1">
            <div class="containinfo">
              <h3 class="main info">Curriculum Vitae</h3>
              <p class="sub info">
                My most recent and up to date copy of my Curriculum Vitae
              </p>
            </div>
            <div class="divider"></div>
            <div class="download">
              <a
                href="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/seth_tobias_cv.pdf"
                download
                class="btn"
                target="blank"
                >Download</a
              >
            </div>
          </div>
          <div class="ditem 2">
            <div class="containinfo">
              <h3 class="main info">Fullstack Web Development Certificate</h3>
              <p class="sub info">
                Certificate of completion of 6 month long Fullstack web dev
                bootcamp.
              </p>
            </div>
            <div class="divider"></div>
            <div class="download">
              <a
                href="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/lc_academy_certificate_st.png"
                download
                class="btn"
                target="blank"
                >Download</a
              >
            </div>
          </div>
          <div class="ditem 3">
            <div class="info">
              <h3 class="main info">National Senior Certificate</h3>
              <p class="sub info">National Senior Certificate.</p>
            </div>
            <div class="divider"></div>
            <div class="download">
              <a
                href="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/nsc_st.png"
                download
                class="btn"
                target="blank"
                >Download</a
              >
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="skills">
      <a name="credentials"></a>
      <a name="skills"></a>
      <div class="container skills">
        <div class="heading">
          <h2>My Skills</h2>
          <div class="line"></div>
        </div>
        <div class="skills">
          <div class="skill start">
            <p class="sback">01</p>
            <h3 class="shead">HTML</h3>
            <p class="sbody">
              I've got seven months of HTML experience and I'm eager to level up
              my skills by diving into advanced techniques and integrating HTML
              with other web technologies.
            </p>
          </div>

          <div class="skill end">
            <p class="sback">02</p>
            <h3 class="shead">CSS</h3>
            <p class="sbody">
              I've got seven months of HTML experience and I'm eager to level up
              my skills by diving into advanced techniques and integrating HTML
              with other web technologies.
            </p>
          </div>
          <div class="skill start">
            <p class="sback">03</p>
            <h3 class="shead">Bootstrap</h3>
            <p class="sbody">
              I've got seven months of HTML experience and I'm eager to level up
              my skills by diving into advanced techniques and integrating HTML
              with other web technologies.
            </p>
          </div>
          <div class="skill end">
            <p class="sback">04</p>
            <h3 class="shead">JavaScript</h3>
            <p class="sbody">
              I've got seven months of HTML experience and I'm eager to level up
              my skills by diving into advanced techniques and integrating HTML
              with other web technologies.
            </p>
          </div>
          <div class="skill start">
            <p class="sback">05</p>
            <h3 class="shead">Vue.js</h3>
            <p class="sbody">
              I've got seven months of HTML experience and I'm eager to level up
              my skills by diving into advanced techniques and integrating HTML
              with other web technologies.
            </p>
          </div>
          <div class="skill end">
            <p class="sback">06</p>
            <h3 class="shead">Node.js</h3>
            <p class="sbody">
              I've got seven months of HTML experience and I'm eager to level up
              my skills by diving into advanced techniques and integrating HTML
              with other web technologies.
            </p>
          </div>
          <div class="skill start">
            <p class="sback">07</p>
            <h3 class="shead">MySQL</h3>
            <p class="sbody">
              I've got seven months of HTML experience and I'm eager to level up
              my skills by diving into advanced techniques and integrating HTML
              with other web technologies.
            </p>
          </div>
          <div class="skill end">
            <p class="sback">08</p>
            <h3 class="shead">GitHub</h3>
            <p class="sbody">
              I've got seven months of HTML experience and I'm eager to level up
              my skills by diving into advanced techniques and integrating HTML
              with other web technologies.
            </p>
          </div>
          <div class="skill start">
            <p class="sback">09</p>
            <h3 class="shead">Docker</h3>
            <p class="sbody">
              I've got seven months of HTML experience and I'm eager to level up
              my skills by diving into advanced techniques and integrating HTML
              with other web technologies.
            </p>
          </div>
          <div class="skill end">
            <p class="sback">10</p>
            <h3 class="shead">Wordpress</h3>
            <p class="sbody">
              I've got seven months of HTML experience and I'm eager to level up
              my skills by diving into advanced techniques and integrating HTML
              with other web technologies.
            </p>
          </div>
          <div class="skill start">
            <p class="sback">11</p>
            <h3 class="shead">Drupal</h3>
            <p class="sbody">
              I've got seven months of HTML experience and I'm eager to level up
              my skills by diving into advanced techniques and integrating HTML
              with other web technologies.
            </p>
          </div>
          <div class="skill end">
            <p class="sback">12</p>
            <h3 class="shead">jQuery</h3>
            <p class="sbody">
              I've got seven months of HTML experience and I'm eager to level up
              my skills by diving into advanced techniques and integrating HTML
              with other web technologies.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section id="certifications">
      <a name="certifications"></a>
      <div class="container certifications">
        <div class="heading">
          <h2>Certifications</h2>
          <div class="line"></div>
        </div>
        <div class="certificate grid">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/APIs.png"
            alt=""
            class="certificate img end"
          />
          <div class="certificate info end">
            <h3>API</h3>
            <p>
              During my time at LC Studios, we underwent comprehensive training
              on the Scrum methodology, utilizing the Agile framework to
              meticulously craft a project proposal for a prospective e-commerce
              platform tailored to client specifications.
            </p>
            <!-- <a href="" class="btn"> Learn More </a> -->
          </div>
        </div>
        <div class="certificate grid">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/Drupal.png"
            alt=""
            class="certificate img start"
          />
          <div class="certificate info start">
            <h3>Drupal</h3>
            <p>
              During my tenure at LC Studios, we underwent comprehensive
              training on the Scrum methodology, utilizing the Agile framework
              to meticulously craft a project proposal for a prospective
              e-commerce platform tailored to client specifications.
            </p>
            <!-- <a href="" class="btn"> Learn More </a> -->
          </div>
        </div>
        <div class="certificate grid">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/hubspot_certificate.png"
            alt=""
            class="certificate img end"
          />
          <div class="certificate info end">
            <h3>SEO Principles</h3>
            <p>
              During my time at LC Studios, we underwent comprehensive training
              on the Scrum methodology, utilizing the Agile framework to
              meticulously craft a project proposal for a prospective e-commerce
              platform tailored to client specifications.
            </p>
            <!-- <a href="" class="btn"> Learn More </a> -->
          </div>
        </div>
        <div class="certificate grid">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/seth-tobias_semrush_certification.jpg"
            alt=""
            class="certificate img start"
          />
          <div class="certificate info start">
            <h3>SEO</h3>
            <p>
              During my tenure at LC Studios, we underwent comprehensive
              training on the Scrum methodology, utilizing the Agile framework
              to meticulously craft a project proposal for a prospective
              e-commerce platform tailored to client specifications.
            </p>
            <!-- <a href="" class="btn"> Learn More </a> -->
          </div>
        </div>
        <div class="certificate grid">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/docker-essentials-a-developer-introduction.png"
            alt=""
            class="certificate img end"
          />
          <div class="certificate info end">
            <h3>Docker</h3>
            <p>
              During my time at LC Studios, we underwent comprehensive training
              on the Scrum methodology, utilizing the Agile framework to
              meticulously craft a project proposal for a prospective e-commerce
              platform tailored to client specifications.
            </p>
            <!-- <a href="" class="btn"> Learn More </a> -->
          </div>
        </div>
        <div class="certificate grid">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/docker_certificate.jpg"
            alt=""
            class="certificate img start"
          />
          <div class="certificate info start">
            <h3>Docker</h3>
            <p>
              During my tenure at LC Studios, we underwent comprehensive
              training on the Scrum methodology, utilizing the Agile framework
              to meticulously craft a project proposal for a prospective
              e-commerce platform tailored to client specifications.
            </p>
            <!-- <a href="" class="btn"> Learn More </a> -->
          </div>
        </div>
        <div class="certificate grid">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/python_certificate.png"
            alt=""
            class="certificate img end"
          />
          <div class="certificate info end">
            <h3>Python</h3>
            <p>
              During my time at LC Studios, we underwent comprehensive training
              on the Scrum methodology, utilizing the Agile framework to
              meticulously craft a project proposal for a prospective e-commerce
              platform tailored to client specifications.
            </p>
            <!-- <a href="" class="btn"> Learn More </a> -->
          </div>
        </div>
        <div class="certificate grid">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/Figma.png"
            alt=""
            class="certificate img start"
          />
          <div class="certificate info start">
            <h3>Figma</h3>
            <p>
              During my tenure at LC Studios, we underwent comprehensive
              training on the Scrum methodology, utilizing the Agile framework
              to meticulously craft a project proposal for a prospective
              e-commerce platform tailored to client specifications.
            </p>
            <!-- <a href="" class="btn"> Learn More </a> -->
          </div>
        </div>
        <div class="certificate grid">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/devops_certificate.png"
            alt=""
            class="certificate img end"
          />
          <div class="certificate info end">
            <h3>DevOps</h3>
            <p>
              During my time at LC Studios, we underwent comprehensive training
              on the Scrum methodology, utilizing the Agile framework to
              meticulously craft a project proposal for a prospective e-commerce
              platform tailored to client specifications.
            </p>
            <!-- <a href="" class="btn"> Learn More </a> -->
          </div>
        </div>
        <div class="certificate grid">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/SCRUM.png"
            alt=""
            class="certificate img start"
          />
          <div class="certificate info start">
            <h3>Scrum</h3>
            <p>
              During my tenure at LC Studios, we underwent comprehensive
              training on the Scrum methodology, utilizing the Agile framework
              to meticulously craft a project proposal for a prospective
              e-commerce platform tailored to client specifications.
            </p>
            <!-- <a href="" class="btn"> Learn More </a> -->
          </div>
        </div>
        <div class="certificate grid">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/ui_certificate.png"
            alt=""
            class="certificate img end"
          />
          <div class="certificate info end">
            <h3>UI/UX</h3>
            <p>
              During my time at LC Studios, we underwent comprehensive training
              on the Scrum methodology, utilizing the Agile framework to
              meticulously craft a project proposal for a prospective e-commerce
              platform tailored to client specifications.
            </p>
            <!-- <a href="" class="btn"> Learn More </a> -->
          </div>
        </div>
        <div class="certificate grid">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/git_certificate.png"
            alt=""
            class="certificate img start"
          />
          <div class="certificate info start">
            <h3>Git & GitHub</h3>
            <p>
              During my tenure at LC Studios, we underwent comprehensive
              training on the Scrum methodology, utilizing the Agile framework
              to meticulously craft a project proposal for a prospective
              e-commerce platform tailored to client specifications.
            </p>
            <!-- <a href="" class="btn"> Learn More </a> -->
          </div>
        </div>
      </div>
    </section>

    <section id="references">
      <a name="references"></a>
      <div class="container references">
        <div class="heading">
          <h2>References</h2>
          <div class="line"></div>
        </div>
        <div class="nav-container">
          <div class="carousel-item-indicator previous" @click="nextItem(-1)">
            <i
              class="fa-solid fa-circle-chevron-left fa-2xl"
              style="color: var(--background)"
            ></i>
          </div>
          <div class="link-items-testimonial" id="one">
            <div class="card1 testimonial-card">
              <div class="card1 container-grid">
                <div class="card1 img-container">
                  <img
                    src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/Ty_Headshot.jpg"
                    alt=""
                  />
                </div>
                <div class="card1 description">
                  <div class="card1 description-collapsed">
                    <div class="card1 description-collapsed-content">
                      <p>Tyheisha Johnson</p>
                    </div>
                    <div class="card1 description-collapsed-content">
                      <p>
                        <a href="https://vue-tj-portfolio.web.app/"
                          >Portfolio</a
                        >
                        |
                        <a href="https://www.linkedin.com/in/tyhieshajohnson/"
                          >Linkedin</a
                        >
                      </p>
                    </div>
                  </div>
                  <div class="card1 description-expanded">
                    <p>
                      Seth is a charismatic and generous person, he connects
                      with everyone in the room. He's analytical and provides
                      help whenever he can. He's determined to achieve the best
                      out of everyday and motivates those around him as well.
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="link-items-testimonial" id="two">
            <div class="card2 testimonial-card">
              <div class="card2 container-grid">
                <div class="card2 img-container">
                  <img
                    src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/Veronique_Headshot.jpg"
                    alt=""
                  />
                </div>
                <div class="card2 description">
                  <div class="card2 description-collapsed">
                    <div class="card2 description-collapsed-content">
                      <p>Veronique Nappie</p>
                    </div>
                    <div class="card2 description-collapsed-content">
                      <p>
                        <a
                          href="https://veroniquex1.github.io/vnappiePortfolio/"
                          >Portfolio</a
                        >
                        |
                        <a
                          href="https://www.linkedin.com/in/veronique-nappie-x1/"
                          >Linkedin</a
                        >
                      </p>
                    </div>
                  </div>
                  <div class="card2 description-expanded">
                    <p>
                      Seth Tobias is both kind and compassionate. The atmosphere
                      that he brings into one's presence is calming and
                      comforting. He has the ability to brighten anyone's day.
                      Seth's work ethic and determination is admirable and
                      inspirational.
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="link-items-testimonial" id="three">
            <div class="card3 testimonial-card">
              <div class="card3 container-grid">
                <div class="card3 img-container">
                  <img
                    src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/Zubaidah_Headshot.jpg"
                    alt=""
                  />
                </div>
                <div class="card3 description">
                  <div class="card3 description-collapsed">
                    <div class="card3 description-collapsed-content">
                      <p>Zubaidah Isaacs</p>
                    </div>
                    <div class="card3 description-collapsed-content">
                      <p>
                        <a href="https://zubaidah-isaacs.web.app/">Portfolio</a>
                        |
                        <a
                          href="https://www.linkedin.com/in/zubaidah-isaacs-1b8070281/"
                          >Linkedin</a
                        >
                      </p>
                    </div>
                  </div>
                  <div class="card3 description-expanded">
                    <p>
                      Seth is a very friendly person and is very committed to
                      his work. He is very hardworking and has good social
                      skills and is good at problem-solving and very
                      enthusiastic too.
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="link-items-testimonial" id="four">
            <div class="card4 testimonial-card">
              <div class="card4 container-grid">
                <div class="card4 img-container">
                  <img
                    src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/Ntokozo_Headshot.jpg"
                    alt=""
                  />
                </div>
                <div class="card4 description">
                  <div class="card4 description-collapsed">
                    <div class="card4 description-collapsed-content">
                      <p>Ntokozo Sithebe</p>
                    </div>
                    <div class="card4 description-collapsed-content">
                      <p>
                        <a href="https://ntoky28.wixstudio.io/myportfolio"
                          >Portfolio</a
                        >
                        |
                        <a href="https://www.linkedin.com/in/ntokozo-sithebe-/"
                          >Linkedin</a
                        >
                      </p>
                    </div>
                  </div>
                  <div class="card4 description-expanded">
                    <p>
                      Seth is a very enthusiastic about life. Everything he
                      talks about has life or character. He is like a sunflower,
                      always blossoming.
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="link-items-testimonial" id="five">
            <div class="card5 testimonial-card">
              <div class="card5 container-grid">
                <div class="card5 img-container">
                  <img
                    src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/Naeema_Headshot.jpg"
                    alt=""
                  />
                </div>

                <div class="card5 description">
                  <div class="card5 description-collapsed">
                    <div class="card5 description-collapsed-content">
                      <p>Naeema Omar</p>
                    </div>
                    <div class="card5 description-collapsed-content">
                      <p>
                        <a href="https://the-portfolio-d6cd8.web.app/"
                          >Portfolio</a
                        >
                        |
                        <a
                          href="https://www.linkedin.com/in/naeema-omar-7ab486299/"
                          >Linkedin</a
                        >
                      </p>
                    </div>
                  </div>
                  <div class="card5 description-expanded">
                    <p>
                      Seth Tobias always brings great energy to the team. He has
                      solid attention to detail which is why he is often
                      designated as our go-to debugger. He is self-driven and
                      always go above and beyond with any task he's given.
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="carousel-item-indicator next" @click="nextItem(1)">
            <i
              class="fa-solid fa-circle-chevron-right fa-2xl"
              style="color: var(--background)"
            ></i>
          </div>
        </div>
        <!-- <div class="ref grid">
          <i class="fa-solid fa-caret-left"></i>
          <div class="ref content 1">
            <div class="ref img">
              <img
                src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/Ty_Headshot.jpg"
                alt=""
                class="reference img"
              />
            </div>

            <div class="ref info">
              <p>
                Seth is a charismatic and generous person, he connects with
                everyone in the room. He's analytical and provides help whenever
                he can. He's determined to achieve the best out of everyday and
                motivates those around him as well.
              </p>
              <p>
                <span> Tyhiesha Johnson </span>: Intern at LC Studio |
                <a href="">Linkedin</a>
              </p>
            </div>
          </div>
          <i class="fa-solid fa-caret-right"></i>
        </div> -->
      </div>
    </section>

    <section id="contact">
      <a name="contact"></a>
      <div class="container contact">
        <div class="heading">
          <h2>Contact</h2>
          <div class="line"></div>
        </div>
        <div class="form flex">
          <div class="details">
            <p>Table View, Cape Town, South Africa</p>
            <a href="">065 887 9439</a>
            <a href="">seth.adams1107@gmail.com</a>
            <a href="">linkedin.com/in/seth-tobias</a>
            <a href="">github.com/SethTobias</a>
            <p>Avaliable @ 08:00 am - 5:30 pm, Monday to Sunday.</p>
          </div>
          <form action="">
            <input type="text" placeholder="Full Name" />
            <input type="text" placeholder="Exammple@EmailAddress.com" />
            <input type="text" placeholder="Phone Number" />
            <input type="text" placeholder="Any Last Comments" />
            <button type="submit">Contact Me</button>
          </form>
        </div>
      </div>
    </section>

    <section id="footer"></section>
  </main>
</template>

<script>
import CertModal from "@/components/CertModal.vue";
import ProjectModal from "@/components/ProjectModal.vue";

export default {
  name: "HomeView",
  components: {
    CertModal,
    ProjectModal,
  },
  data() {
    return {
      carouselIndex: 1,
      isModalVisible: false,
      modalTitle: "",
      modalMsg: "",
      modalGit: "",
      modalLink: "",
    };
  },
  methods: {
    carouselSetItem() {
      return this.carouselIndex;
    },
    displayItem(n) {
      let c = 0;
      let carouselItems = document.querySelectorAll(".link-items-testimonial");
      if (n > carouselItems.length) {
        this.carouselIndex = 1;
      }
      if (n < 1) {
        this.carouselIndex = carouselItems.length;
      }
      for (c = 0; c < carouselItems.length; c++) {
        carouselItems[c].style.display = "none";
      }
      carouselItems[this.carouselIndex - 1].style.display = "flex";
    },
    currentItem(n) {
      this.displayItem(this.carouselIndex);
    },
    nextItem(n) {
      this.displayItem((this.carouselIndex += n));
    },
    openModal(title, msg) {
      this.modalTitle = title;
      this.modalMsg = msg;
      this.modalGit = github;
      this.modalLink = link;
      this.isModalVisible = true;
    },
    closeModal() {
      this.isModalVisible = false;
      this.modalTitle = "";
      this.modalMsg = "";
      this.modalGit = "";
      this.modalLink = "";
    },
  },
};
</script>
<style>
main {
  position: absolute;
  right: 0;
  top: 0;
  width: 75%;
  padding: 0;
}

section {
  background-color: blue;
  border: solid 10px black;
  border-left: 0;
  border-right: 0;
}

.container {
  background-color: brown;
  width: 65vw;
  margin: 0 auto;
  padding: 25px 0;
}

.heading {
  margin-bottom: 25px;
}

.heading h2 {
  margin-top: 0;
  margin-bottom: 0;
  text-align: center;
}

.line {
  border-bottom: solid white 5px;
}

.img {
  height: auto;
}

.btn {
  border: 2px blue solid;
  text-decoration: none;
  color: whitesmoke;
  padding: 5px;
  width: fit-content;
}

.btn.end {
  align-self: end;
}

#landing {
  display: grid;
  grid: 1fr / 1fr;
  place-items: center;
  text-align: center;
  padding: 0;
}

#landing div {
  grid-area: 1/1/2/2;
  z-index: 1;
}

.landing {
  width: 100%;
  height: 100vh;
  object-fit: cover;
  grid-area: 1/1/2/2;
}

#about {
}

.container.about {
}

.container.about .heading {
}

.content.about {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.content.about p {
  margin: 0;
  max-height: 400px;
  max-width: 400px;
}

.container.about .about-img {
  max-width: 350px;
  max-height: 450px;
}

.img.about {
  height: 100%;
  width: 100%;
  object-fit: fill;
}

#projects {
}

.project:hover {
  cursor: pointer;
}

ul {
  list-style-type: none;
  padding: 0;
}
li {
  cursor: pointer;
  margin: 5px 0;
}

.container.projects .projects {
  display: grid;
  gap: 10px;
  grid:
    "pro1 pro1 pro2" 125px
    "pro1 pro1 pro3" 125px
    /* "pro4 pro6 pro6" 150px 
    "pro5 pro6 pro6" 150px  */
    / 1fr 1fr 0.9fr;
}

.container.projects .heading {
}

.project {
  background-color: grey;
}

.project img {
  height: 100%;
  width: 100%;
  object-fit: cover;
}

.project.one {
  grid-area: pro1;
}

.project.two {
  grid-area: pro2;
}

.project.three {
  grid-area: pro3;
}
/* .project.four {
  grid-area: pro4;
}

.project.five {
  grid-area: pro5;
}

.project.six {
  grid-area: pro6;
} */

#experience {
}

.container.experience {
  display: flex;
  flex-direction: column;
  align-content: center;
  justify-content: center;
}

.item {
  display: grid;
  grid: "txt line img" 300px / 1fr 100px 1fr;
  place-items: center;
}

.time-text {
  grid-area: txt;
}
.time-text h3 {
  margin-top: 0;
}

.time-line {
  grid-area: line;
  display: grid;
  grid: 20px 50px 230px / 100%;
}

.time-line p {
  text-align: center;
  margin: 0;
  z-index: 1;
  grid-area: 1/1/2/2;
}

.time-line i {
  grid-area: 2/1/3/2;
  background-color: cornflowerblue;
  width: 50px;
  height: 50px;
  font-size: 30px;
  text-align: center;
  margin: 0 auto;
  z-index: 1;
  display: flex;
  align-items: center;
  justify-content: center;
  border: black 1px solid;
  border-radius: 100%;
}

.time-line div {
  grid-area: 1/1/4/2;
  background-color: darkblue;
  width: 10px;
  height: 100%;
  margin: 0 auto;
  border-top-left-radius: 25px;
  border-top-right-radius: 25px;
}

.container.experience .time-line div {
  border-bottom-left-radius: 25px;
  border-bottom-right-radius: 25px;
}

.time-img {
  grid-area: img;
}
.time-img img {
  width: 100%;
  height: 80%;
  object-fit: cover;
}

#education {
}

.container.education {
  display: flex;
  flex-direction: column;
  align-content: center;
  justify-content: center;
}

.item.two {
  display: grid;
  grid: "img line txt" 300px / 1fr 100px 1fr;
  margin-top: 0px;
}

.item.two .time-line div {
  border-radius: 0;
  border-bottom-left-radius: 25px;
  border-bottom-right-radius: 25px;
}

.item.two .time-text {
  text-align: right;
}

#r_resources {
}

.container.resources {
  background-color: gray;
}

.downloads {
  display: flex;
  flex-direction: column;
  width: 40vw;
  margin: 0 auto;
  /* justify-content: center;
  align-content: center; */
}

.ditem {
  display: grid;
  grid: "info divider btn" 1fr/ 4fr 0.25fr 1fr;
  /* margin: 0 auto; */
}

.bivider {
  border-right: 1px grey solid;
  height: 65%;
  margin: auto;
}

.download {
  display: flex;
  /* margin: auto 0; */
  justify-content: center;
  align-items: center;
}

#skills {
}

.skills {
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.skill.start {
  /* height: 300px; */
}
.skill.end {
  /* height: 300px; */
}

.skill {
  /* width: 25vw; */
  /* height: 38vh; */
  display: grid;
  grid: 25px 100px / 5vw 5vw 15vw 15vw;
}

.sback {
  grid-area: 1/1/3/3;
  font-size: 2.5rem;
  align-self: center;
  /* z-index: -1; */
}

.shead {
  grid-area: 1/2/2/3;
  z-index: 1;
}

.sbody {
  grid-area: 2/2/3/5;
}

.skill.start {
  align-self: flex-start;
}

.skill.end {
  align-self: flex-end;
}

#certifications {
}

.certificate.grid {
  display: grid;
  grid: 1fr / 1fr 4fr;
  column-gap: 50px;
  margin-top: 50px;
}

.certificate.img {
  width: 200px;
  height: auto;
}

.certificate.img.start {
  grid-area: 1/1/1/2;
}

.certificate.img.end {
  grid-area: 1/5/1/6;
}

.certificate.info {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.certificate.info :where(h3, p) {
  margin: 0;
}

.certificate.info.start {
  grid-area: 1/2/1/6;
}

.certificate.info.end {
  grid-area: 1/1/1/5;
}

#references {
}

.carousel-main-container {
  /* max-width: 1000px; */
  position: relative;
  margin: 0 auto;
}
.carousel-item {
  display: none;
}

.testimonial-container {
  margin: 0 auto;
  /* width: 1250px; */
  margin-bottom: 25px;
}

.carousel-item-indicators {
  cursor: pointer;
  position: absolute;
  display: flex;
  place-content: center space-evenly;
  user-select: none;
}
.carousel-item-indicator.previous,
.carousel-item-indicator.next {
  cursor: pointer;
  z-index: 1;
  align-content: center;
}
.carousel-item-index {
  position: absolute;
  top: 0;
  left: 0;
}

.nav-container {
  display: flex;
  /* justify-content: space-between; */
  align-items: center;
  width: 65vw;
  background-color: grey;
  text-align: center;
}

.link-items-testimonial {
  width: 60vw;
}

:has(.link-items-testimonial) :where(#two, #three, #four, #five) {
  display: none;
}

.nav-link {
  margin: 0 auto;
  display: flex;
  align-content: center;
  justify-content: space-between;
  /* max-width: 1250px;
  width: 1250px;
  min-width: 250px; */
}

.testimonial-card {
  /* background-color: var(--secondary); */
  height: fit-content;
  width: fit-content;
  /* border: 7.5px groove var(--text); */
  margin: 10px auto;
  justify-content: center;
}
.testimonial-card:hover {
  /* border-color: var(--secondary); */
}
.link-items-testimonial.one .testimonial-items1,
.link-items-testimonial.two .testimonial-items2 {
  /* grid-area: 1/1/2/2; */
  /* width: 1200px; */
  display: flex;
  flex-flow: row wrap;
  justify-content: space-evenly;
}

.testimonial-items1 .testimonial-card {
  /* background-color: var(--secondary); */
}

.container-grid {
  /* height: 320px; */
  /* width: 350px; */
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.img-container {
  grid-area: img;
}

.img-container img {
  width: 350px;
  height: auto;
}

.testimonial-items1 .description,
.testimonial-items2 .description {
  grid-area: description;
  background-color: var(--primary);
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
  font-size: 1.1rem;
}

/* .description-collapsed-content {
  text-align: center;
} */

/* .description-expanded {
  text-align: center;
  padding: 0 25px;
  font-size: 1rem;
}
.testimonial-items1 .description-expanded,
.testimonial-items2 .description-expanded {
  overflow: hidden;
} */

/* .testimonial-items2 {
  grid-area: 1/1/2/2;
  display: flex;
  flex-flow: row wrap;
  justify-content: space-evenly;
}

.testimonial-items2 .testimonial-card {
  background-color: var(--primary);
} */

@media screen and (max-width: 300px) {
  .carousel-main-container {
    width: 300px;
  }
  .carousel-item {
    display: none;
  }
  .carousel-item-indicators.next,
  .carousel-item-indicators.previous {
    width: 25px;
  }
  .carousel-item-indicator.next i,
  .carousel-item-indicator.previous i {
    font-size: 25px;
  }

  .link-items-testimonial.two {
    display: none;
  }
  .nav-link {
    margin: 0 auto;
    display: flex;
    align-content: center;
    justify-content: space-between;
    width: 250px;
  }

  .testimonial-container {
    margin: 0 auto;
    width: 250px;
  }

  h2 {
    font-size: 1.5rem;
  }

  .testimonial-card {
    background-color: var(--secondary);
    height: fit-content;
    width: fit-content;
    margin: 10px auto;
  }
  .link-items-testimonial.one .testimonial-items1,
  .link-items-testimonial.two .testimonial-items2 {
    /* grid-area: 1/1/2/2; */
    width: 250px;
    display: flex;
    flex-flow: row wrap;
    justify-content: space-evenly;
  }

  .container-grid {
    height: 250px;
    width: 200px;
  }

  .testimonial-items1 .description,
  .testimonial-items2 .description {
    font-size: 0.75rem;
  }

  .description-expanded {
    font-size: 0.7rem;
  }

  .testimonial-items2 {
    flex-flow: column;
    justify-content: space-evenly;
    margin: 10px auto;
  }
}

#contact {
}

.form.flex {
  display: flex;
  justify-content: space-around;
}

.details {
  display: flex;
  flex-direction: column;
}

form {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  width: 200px;
}

#footer {
  background-color: white;
  height: 75px;
}
</style>
