### Hello camille,

## Please read this file to easily manipulate the template pages.

## This is a module structure i've built to help you easily make changes:

1 - First copy the first.html page and create a new page for a template project in the projects folder (eg: project.html).

2 - past the content in the newly created page.

3 - change page title in the Head element only.

4 - In the main html tag, the first section change the hero text content after that section there is the main image change only it's src attribut to the one that you want.

5 - now you have the "template-section" basically all changebale section:
-- If you want you can add below the "section-description" tags like this :

            <div class="tag-box">
              <span class="tag">Wireframes</span>
              <span class="tag">Prototypes</span>
            </div>

-- If you want you can add below that an img or multiple imgs like this :

          <img
            src="../assets/page images/image-2@2x.png"
            alt="design of anna money app by camille brunette"
            class="section-img"
          />

-- If you want you can add below the image a block of text and it is optional to have tags block too, like this :

          <div class="details-box">
            <div class="text-box">
              <p class="text-box--title">VAT Return Filing</p>
              <p class="text-box--description">
                Using a direct link to HMRC and with all of these great features
                and even I did some copywriting here. I created wireframes, and
                I worked with a UI designer who finalised the appearance.
              </p>
            </div>
            <div class="tag-box">
              <span class="tag">Wireframes</span>
              <span class="tag">Prototypes</span>
            </div>
          </div>

-- If you want you can add a block of 2 Image side by side, like this :

          <div class="double-imgs">
            <img
              src="../assets/page images/image-6@2x.png"
              alt="design of anna money app by camille brunette"
              class="section-img"
            />
            <img
              src="../assets/page images/image-7@2x.png"
              alt="design of anna money app by camille brunette"
              class="section-img"
            />
          </div>

6 - Now you can create multiple sections in this way.

7 - Just leave the rest (portfolio & footer) as it is, just make sure to update projects urls.

8 - Also make sure to update projects urls in home page & portfolio page.

9 - Overall, even without this the code is self explanatory.

10 - If you want to (add, modify, delete) animations just add this code to the element you want:

    <div data-aos="fade-right" data-aos-duration="1000">
      <span class="tag">Wireframes</span>
      <span class="tag">Prototypes</span>
    </div>

-- don't do fade-left, it my produce bugs.
-- You can always check their library page: https://michalsnik.github.io/aos/

See you next time 👋

/////////////////////////////////////////////////////////////
--- Camille Portfolio Updated version: ---
/////////////////////////////////////////////////////////////

1 - For the Highlights, you add a similar block inside of a section-container:
--- If you want a background, add highlights-bg alongise the class template-section div.

    <div class="highlights-box">
      <div>
        <img src="./assets/new images/highlight-1.png" />
        <div>
            <p class="highlight-title">Project metrics</p>
              <div class="highlights-desc">
                <p>
                  There were two key metrics we would chase on this project:
                </p>
              </div>
          </div>
      </div> --> a div for each highlight block
    </div>
    <div class="summary">
        <p class="summary-title">Time frame</p>
        <p class="summary-paragraph">
          We spent a total of 3 months on the design phase of this project.
          To fully engineer the solution and have it released took another 2
          months.
        </p>
      </div>

2 - For the 70/30 components, you do it like this:

        <div> ---> this div can contain multiple comps
            <div class="f-layout">
              <img src="./assets/new images/additional-research.png" />
              <div class="f-layout--box">
                <p class="f-layout--title">Additional research interviews</p>
                <div class="f-layout--text">
                  <p>
                    To deep-dive on pain points, I contacted customers in our
                    customer base and asked them a few questions regarding their
                    perspective on payroll.
                  </p>
                  <p>Some specific problems came out of the conversations.</p>
                </div>
              </div>
            </div>
            <!--  -->

          </div>
        </div>

3 - For the Banner components, you do it like this:
-- also just add your banner inside the template-container:

          <div class="banner banner-blue">
            <p class="banner-title">Who is our user?</p>
            <!--  -->
            <div class="banner-feature">
              <img src="./assets/new images/icon-bag.png" />
              <div>
                <span class="icon-title">Motivations</span>
                <span class="banner-text">
                  &mdash; Freeing up time to spend with the family, upskilling
                  to be more self-sufficient as a business owner. Saving on
                  costs.
                </span>
              </div>
            </div>
          </div>

-- for the banner color, add classes: banner-blue, banner-orange, banner-grey.

4 - For the 2-up blocks component, you do it like this:
--also, just add it inside your template-container

          <div class="double-blocks">
            <div>
              <img
                src="./assets/new images/competitive-1.png"
                class="section-img"
              />
              <p class="double-blocks--title">Competitive matrix</p>
              <p class="double-blocks--text">
                The Product Owner mapped out competitors and their feature set
                in a matrix.
              </p>
            </div>
            <div>
              <img
                src="./assets/new images/competitive-2.png"
                class="section-img"
              />
              <p class="double-blocks--title">Competitor deep dive</p>
              <p class="double-blocks--text">
                I researched products by trialing their platform or taking part
                in demos. Luckily, I needed a live tool for my own business, so
                it was great to connect with market offerings.
              </p>
            </div>
          </div>

5 - For the Flowed components, you do it like this:
--also, just add it inside your template-container

          <div class="flowed-component">
            <img src="./assets/new images/workshop.jpg" class="section-img" />
            <div class="text-block">
              <p class="block-title">Crazy 8’s</p>
              <p class="block-text">
                I led the small team in a Crazy 8 exercise, conducting idea
                generation on what a minimum viable product might look like,
                having users onboard, use a simple experience and subscribe to
                pay.
              </p>
            </div>
            <div class="text-block">
              <p class="block-title">Affinity mapping</p>
              <p class="block-text">
                I took our ideas and organised them with the group using sticky
                notes (top right). This helped us identify our key ideas.
              </p>
            </div>
            <div class="text-block">
              <p class="block-title">Sketching a high level flow</p>
              <p class="block-text">
                Taking our key ideas, we established as a group a high level
                user flow and the experiences that users would interact with
                (bottom right). This formed a hypothesis for our MVP.
              </p>
            </div>
          </div>

6 - For the Text under image components, you do it like this:
--also, just add it inside your template-container

          <div class="img-text-block">
            <img
              src="./assets/new images/user-journeys.png"
              class="section-img"
            />
            <div class="text-block">
              <p class="block-title">User Journeys</p>
              <p class="block-text">
                I outlined the steps users would take to complete payroll tasks.
                The product owner and engineering lead approved these before
                moving to the next step. They served as a great understanding
                for everyone to grasp and collaborate on what we would be
                building.
              </p>
              <br />
              <br />
              <p class="block-text">
                I outlined the steps users would take to complete payroll tasks.
                The product owner and engineering lead approved these before
                moving to the next step. They served as a great understanding
                for everyone to grasp and collaborate on what we would be
                building.
              </p>
            </div>
          </div>

7 - For the tag, just put it on top inside the template-container
