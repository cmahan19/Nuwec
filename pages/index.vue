<template>
  <v-app dark
    :style="{ backgroundImage: 'url(@/assets/images/OIP.jpg)', backgroundSize: 'cover', backgroundPosition: 'center', backgroundRepeat: 'no-repeat', padding: 0 }">
    <v-container fluid>
      <v-row>
        <v-col cols="12">
          <v-carousel height="300" width="100%" :cycle="true">

            <v-carousel-item>
              <img src="@/assets/images/data2.jpg" alt="Image 1" class="flex-shrink-0" width="100%" height="100%" object-fit="cover">
              <v-overlay>
                <v-container fluid>
                  <v-card-text class="text-center">
                    <div class="h1-container">
                        <span>Nuwec</span>
                      </div>
                    <p :style="{ marginTop: '10px' }">Nuwec Your certified partner in IT services and data management. We help businesses of all sizes achieve thier data-driven goals.</p>
                    <v-btn color="primary" dark class="mx-auto">Join Us</v-btn>
                  </v-card-text>
                </v-container>
              </v-overlay>
            </v-carousel-item>

            <v-carousel-item>
              <img src="@/assets/images/data1.jpg" alt="Image 1" class="flex-shrink-0" width="100%" height="100%" object-fit="cover">
              <v-overlay>
                <v-container fluid>
                  <v-card-text class="text-center">
                    <div class="h1-container">
                        <span>Nuwec</span>
                      </div>
                    <p :style="{ marginTop: '10px' }">Well-managed data is the bridge between raw information and actionable knowledge.</p>
                    <v-btn color="primary" dark class="mx-auto">Join Us</v-btn>
                  </v-card-text>
                </v-container>
              </v-overlay>
            </v-carousel-item>
            <v-carousel-item>
              <img src="@/assets/images/data3.jpg" alt="Image 1" class="flex-shrink-0" width="100%" height="100%" object-fit="cover">
              <v-overlay>
                <v-container fluid>
                  <v-card-text class="text-center">
                    <div class="h1-container">
                        <span>Nuwec</span>
                      </div>
                    <p :style="{ marginTop: '10px' }">From compliance to efficiency, we empower your growth. Nuwec: Where data fuels innovation and drives tangible results.</p>
                    <v-btn color="primary" dark class="mx-auto">Join Us</v-btn>
                  </v-card-text>
                </v-container>
              </v-overlay>
            </v-carousel-item>

          </v-carousel>
        </v-col>
      </v-row>

      <v-row>
  <v-col cols="12">
    <v-card class="dama-wheel-card" style="display: flex; flex: 1">
      <v-container>
        <iframe width="560" height="315" src="https://www.youtube.com/embed/?rel=0" frameborder="0" allowfullscreen id="player"></iframe>
      </v-container>

      <v-card-text>
        <span>nuwec</span>
        <p style="margin-top: 20px">
          <a href="https://www.un.org/sites/un2.un.org/files/2021/03/udhr.pdf" target="_blank">Nuwec</a> 
        </p>
        <v-btn color="primary" dark class="mx-auto">Join Us</v-btn>
      </v-card-text>
    </v-card>
  </v-col>
</v-row>

<v-row>
        <v-col cols="12">
          <v-card>
            <v-card-title>In today's data-driven world, information has become the new goldrush.</v-card-title>
            <v-card-text>

  <p>Information in its raw form is merely potential. To truly unlock its value, it needs to be transformed into usable, meaningful insights.</p>

  <p> This is where good data management comes in:</p>
  <ul>
    <li>Data cleansing and organization: Raw data is often messy and incomplete. Cleaning, structuring, and organizing it is crucial for accurate analysis and interpretation.</li>
    <li>Data analysis and interpretation: Extracting insights from data requires the right tools and expertise. Skilled data analysts can uncover patterns, trends, and hidden relationships within the data.</li>
    <li>Data visualization and communication: The insights gained from data need to be effectively communicated to stakeholders in a clear and concise way. Data visualization plays a crucial role in making information accessible and actionable.</li>
  </ul>

  <p>Here's why information is such a prized commodity:</p>

  <ul>
    <li>Scarcity: Unlike other resources, information can be infinitely replicated, but true insights and actionable knowledge are scarce. The ability to distill valuable information from the noise is key.</li>
    <li>Decision-making power: Businesses, governments, and individuals rely on information to make informed decisions. Having access to better data means making better choices, gaining a competitive edge, and influencing outcomes.</li>
    <li>Personalization and relevance: The ability to personalize experiences and deliver targeted information is invaluable. Well-managed data allows businesses to understand their customers, target ads effectively, and create relevant content.</li>
    <li>Innovation and knowledge creation: New discoveries and advancements often hinge on the analysis and synthesis of existing information. By managing data effectively, we can unlock new solutions and push the boundaries of knowledge.</li>
  </ul>

  <v-btn color="primary" dark class="mx-auto">Join Us</v-btn>
</v-card-text>

          </v-card>
        </v-col>
      </v-row>

      <v-row>
        <v-col cols="12">
          <v-card class="flex flex-wrap">
            <v-card-title>Events</v-card-title>
            <v-card-text>
              <p>Are you passionate about data</p>

              <p>  Our events will feature a variety of speakers and activities that will explore the many different aspects of human rights. We'll learn about the history of human rights, the challenges that still exist today, and what we can do to make a difference.</p>

              <p> We hope that you'll join us for these important events. Together, we can make South Dakota a more just and equitable place for everyone.</p>
              </v-card-text>
              <v-card-text>
          </v-card-text>
            <v-subheader>Upcoming Events</v-subheader>
            <v-calendar :events="eventList">
              <v-for="event in eventList" :key="event.name" :name="event.name" :start="event.start" :end="event.end"
                :location="event.location" :description="event.description" />
              <!-- <v-link :href="event.registerLink">Register</v-link> -->
              <template v-if="eventList.length === 0">
                <p>There are no upcoming events.</p>
              </template>
            </v-calendar>

          </v-card>
        </v-col>
      </v-row>

      <v-row>
        <v-col cols="12">
          <v-card-title><v-btn color="primary" dark class="mx-auto">Sponsor</v-btn></v-card-title>
          <v-card-text>These companies have demonstrated a high level of commitment to equality. Please consider supporting those that support us.
          </v-card-text>
          <v-carousel height="auto" width="100%" :cycle="true">
            
            <v-carousel-item>
              <v-card class="sponsor-card" style="display: flex; flex: 1" >
      <v-container>
        <img width="25%" height="315" src="@/assets/images/Nuwec.png" frameborder="0" allowfullscreen id="player">
      </v-container>

      <v-card-text>
        <span>Nuwec</span>
        <p style="margin-top: 20px">
          At Nuwec, we believe that data is the key to success in today's digital world. That's why we offer a comprehensive suite of data management and IT services to help clients of all sizes harness the power of their data to drive growth and innovation.
       </p>
      </v-card-text>
    </v-card>
            </v-carousel-item>

            <v-carousel-item>
              <v-card class="sponsor-card" style="display: flex; flex: 1">
      <v-container>
        <img width="25%" height="315" src="@/assets/images/Nuwec.png" frameborder="0" allowfullscreen id="player">
      </v-container>

      <v-card-text>
        <span>Nuwec</span>
        <p style="margin-top: 20px">
          At NuWec, we believe that data is the key to success in today's digital world. That's why we offer a comprehensive suite of data management and IT services to help clients of all sizes harness the power of their data to drive growth and innovation.
       </p>
      </v-card-text>
    </v-card>
            </v-carousel-item>

          </v-carousel>
        </v-col>
      </v-row>

      <v-row>
  <v-col cols="12">
    <v-card>
      <v-card-title>Helpfull Links</v-card-title>
      <v-card-text>
        <v-list>
          <v-list-item link :to="{ href: 'https://www.un.org/en/global-issues/human-rights' }">
            <span>Nuwec</span>
          </v-list-item>
          <v-divider />
          <v-list-item link :to="{ href: 'https://www.humanrights.com/' }">
            <span>Nuwec</span>
          </v-list-item>
          <v-divider />
          <v-list-item link :to="{ href: 'https://www.hrc.org/' }">
            <span>Nuwec</span>
          </v-list-item>
        </v-list>
      </v-card-text>
    </v-card>
  </v-col>
</v-row>


    </v-container>

  </v-app>
</template>

<style>@import '@/assets/style.css';</style>

<script>
export default {
  name: 'CarouselExample',
  data() {
    return {
      eventList: [
        {
          name: 'DAMA International Conference',
          start: '2023-10-16T09:00:00',
          end: '2023-10-18T17:00:00',
          location: 'Las Vegas, NV',
          description: 'The DAMA International Conference is the world\'s largest gathering of data management professionals.'
        },
        {
          name: 'DAMA SD Chapter Meeting',
          start: '2023-10-19T18:00:00',
          end: '2023-10-21T20:00:00',
          location: 'Houston, TX',
          description: 'The DAMA Houston Chapter Meeting is a monthly meeting for data management professionals in the Houston area.'
        }
      ]

    }
  }
}
</script>

