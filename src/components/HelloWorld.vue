<template>
  <div class="top-card">
    <p class="name"><span>A</span>nimesh.</p>
    <div class="social-icons">
      <button class="home-btn" >Home</button>
      <button class="about-btn" @click="goTo('about')">About</button>
      <button class="portfolio-btn" @click="goTo('portfolio')">Portfolio</button>
      <button class="contact-btn" @click="goTo('contact')">Contact</button>
    </div>
  </div>

  <div class="shortintro">
    <p>
      <span class="job">Business Analyst/Developer</span> <br />Hi, I'm
      <span>Animesh</span> <br />
      from India
    </p>
    <img src="@/assets/image.jpg" alt="Animesh" class = "fixed-img"/>
  </div>

  <div class="about" id="about">
    <img src="@/assets/image.jpg" alt="Animesh" />

    <div class="tabs">
      <h1><span>About</span> Me</h1>
      <p>I am a versatile professional with a passion for business analysis and backend development. 
        I have experience in using a variety of tools and languages including Golang, Python, SQL, Power BI, 
        and Excel to create solutions that meet customer and stakeholder needs.
        I enjoy learning about new technology and applying it to solving real-world problems.</p>

      <div class="all-tabs">
        <button class="tab" :class="{ 'active': activeTab === 'skills' }" @click="activeTab = 'skills'">Skills</button>
        <button class="tab" :class="{ 'active': activeTab === 'experience' }" @click="activeTab = 'experience'">Experience</button>
        <button class="tab" :class="{ 'active': activeTab === 'education' }" @click="activeTab = 'education'">Education</button>
        <button class="tab" :class="{ 'active': activeTab === 'certifications' }" @click="activeTab = 'certifications'">Certifications</button>
      </div>

      <div class="tab-contents">

        <div v-show="activeTab === 'skills'" class="tab-content">
          <p><span>Business Analytics</span><br>Microsoft Excel, Python, Power BI, SQL</p>
          <p><span>Backend Developement</span><br>Golang, API</p>
          <p><span>Frontend Developement</span><br>HTML, CSS, Javascript, Vue.Js</p>
        </div>

        <div v-show="activeTab === 'experience'" class="tab-content" >
          <p><span>August 2023 - Current</span><br>Business Analyst/Developer at Enverus</p>
          <p><span>January 2020 - July 2023</span><br>Freelancing at Upwork & Fiverr</p>
        </div>

        <div v-show="activeTab === 'education'" class="tab-content">
          <p><span>August 2019 - August 2023</span><br>B.Tech In Petroleum Engineering from UPES</p>
          <p><span>2015 - 17</span><br>High School Education</p>
        </div>

        <div v-show="activeTab === 'certifications'" class="tab-content cert">




          <div class="cert-div">
              <img src = "https://media.licdn.com/dms/image/C4E0BAQFxFp3CSggmyQ/company-logo_100_100/0/1630585942634/carolyn_test_page_logo?e=1710374400&v=beta&t=c5GlW8mmMzzVu1WFStM0jZAY98gyK7rD_QU_n1DQIzc">
              <p>Enverus Certified Specialist</p>
              <a href="https://learn.enverus.com/c/htaOqYH3TNGedtHwr4lcoA" target=”_blank”>Show Credentials</a>
          </div> 
          <div class="cert-div">
              <img src = "https://media.licdn.com/dms/image/C4E0BAQFxFp3CSggmyQ/company-logo_100_100/0/1630585942634/carolyn_test_page_logo?e=1710374400&v=beta&t=c5GlW8mmMzzVu1WFStM0jZAY98gyK7rD_QU_n1DQIzc">
              <p>Enverus Certified Associate</p>
              <a href="https://learn.enverus.com/c/iTykwtfnQk-f_TNtbAAtog" target=”_blank”>Show Credentials</a>
          </div> 
          <div class="cert-div">
              <img src = "https://media.licdn.com/dms/image/C4E0BAQFGfERBPGurCg/company-logo_100_100/0/1631307390795?e=1710374400&v=beta&t=nTKeIhiFHJmj9l8OCD7iYainktqfXGAubErLk68ji90">
              <p>Programming for everybody</p>
              <a href="https://www.coursera.org/account/accomplishments/records/H7UXPDKGTGCG?utm_source=android&utm_medium=certificate&utm_content=cert_image&utm_campaign=sharing_cta&utm_product=course" target=”_blank”>Show Credentials</a>
          </div> 
          <div class="cert-div">
              <img src="https://media.licdn.com/dms/image/C4D0BAQG12formuFdJg/company-logo_100_100/0/1630469288270/technion_logo?e=1710374400&v=beta&t=UQ0K6cAwz1gYhhyMZ3slZ6rCJPrOakaWxpaRIRyHEao">
              <p>From Idea to startup</p>
              <a href="https://www.coursera.org/account/accomplishments/records/CB8NC2HJKZSK?utm_source=android&utm_medium=certificate&utm_content=cert_image&utm_campaign=sharing_cta&utm_product=course" target=”_blank”>Show Credentials</a>
          </div> 
          <div class="cert-div">
              <img src="https://media.licdn.com/dms/image/D560BAQGiz5ecgpCtkA/company-logo_100_100/0/1688684715866/ibm_logo?e=1710374400&v=beta&t=Furn0vXql4qh6cesBQ3Ncf3zVolROT2u95LMYdmK-L8">
              <p>Introduction to data analytics</p>
              <a href="https://coursera.org/share/5ddd1deb080d92cc4826ef5b65706572" target=”_blank”>Show Credentials</a>
          </div> 
          <div class="cert-div">
              <img src="https://media.licdn.com/dms/image/D560BAQGiz5ecgpCtkA/company-logo_100_100/0/1688684715866/ibm_logo?e=1710374400&v=beta&t=Furn0vXql4qh6cesBQ3Ncf3zVolROT2u95LMYdmK-L8">
              <p>Excel basics for data analytics</p>
              <a href="https://coursera.org/share/5ddd1deb080d92cc4826ef5b65706572" target=”_blank”>Show Credentials</a>
          </div> 
          <div class="cert-div">
              <img src="https://media.licdn.com/dms/image/C560BAQHaVYd13rRz3A/company-logo_100_100/0/1638831590218/linkedin_logo?e=1710374400&v=beta&t=nwehz-T4oKXmlQvGHKME54Pi5eLZN0-Oqh72iPFkggc">
              <p>Learning Go</p>
              <a href="https://www.linkedin.com/learning/certificates/6dbb1aaf3608118e88bd26e62326a457f96b51223c407d429c8d44150dcf2ef3" target=”_blank”>Show Credentials</a>
          </div> 
          <div class="cert-div">
              <img src="https://media.licdn.com/dms/image/C560BAQHaVYd13rRz3A/company-logo_100_100/0/1638831590218/linkedin_logo?e=1710374400&v=beta&t=nwehz-T4oKXmlQvGHKME54Pi5eLZN0-Oqh72iPFkggc">
              <p>Learning Git and GitHub</p>
              <a href="https://www.linkedin.com/learning/certificates/c406119829d9b48175b3a16461e0a54317cf190a9c1b28da92b9afde00f4499e" target=”_blank”>Show Credentials</a>
          </div> 
          <div class="cert-div">
              <img src="https://media.licdn.com/dms/image/C560BAQHaVYd13rRz3A/company-logo_100_100/0/1638831590218/linkedin_logo?e=1710374400&v=beta&t=nwehz-T4oKXmlQvGHKME54Pi5eLZN0-Oqh72iPFkggc">
              <p>Power BI Essential Training</p>
              <a href="https://www.linkedin.com/learning/certificates/4a4f930ca6ad4014e9315af7dae0118b298ddf2603cf72fec228f983fd757746" target=”_blank”>Show Credentials</a>
          </div> 
          <div class="cert-div">
              <img src="https://media.licdn.com/dms/image/C560BAQHaVYd13rRz3A/company-logo_100_100/0/1638831590218/linkedin_logo?e=1710374400&v=beta&t=nwehz-T4oKXmlQvGHKME54Pi5eLZN0-Oqh72iPFkggc">
              <p>Advanced Power BI: DAX Language, Formulas, and Calculations</p>
              <a href="https://www.linkedin.com/learning/certificates/92b13c7ea15738a4fb91ee118f2641a960d61fd39f2916834438adde95d8c529" target=”_blank”>Show Credentials</a>
          </div> 
         

        </div>

      </div>
    </div>
  </div>
  <div class = "portfolio" id="portfolio">
    <h1>Portfolio</h1>
    <p>Coming Soon</p>
  </div>

  <div class = "contact" id="contact">

    <div class="contact-me">
        <h1>Contact Me</h1>
        <div class="mail">
            <img src="@/assets/send-mail.png" />
            <p>animeshsingh161@gmail.com</p>
            
        </div>
        <div class="phone">
            <img src="@/assets/telephone.png" />
            <p>8434451937</p>
            
        </div>
        <div class="social">
            <a href="https://www.linkedin.com/in/animesh-singh-7370/" target=”_blank” ><img src="https://media.licdn.com/dms/image/C560BAQHaVYd13rRz3A/company-logo_100_100/0/1638831590218/linkedin_logo?e=1710374400&v=beta&t=nwehz-T4oKXmlQvGHKME54Pi5eLZN0-Oqh72iPFkggc"></a>
            <a href="https://medium.com/@animeshsingh161" target=”_blank” ><img src="https://media.licdn.com/dms/image/C4D0BAQEv0xgEe3MJ2w/company-logo_200_200/0/1630543048076/medium_com_logo?e=1710374400&v=beta&t=LY5WevOnWlPVdKE3DAd_bEWqghkqcaeBnP9BYqyMj-o"></a>
            
            
        </div>

        <div class="resume">
            <a href="https://drive.google.com/uc?export=download&id=1AFg5vjneAtpBWhwpaaSLQND5kz9vaWAx" download>Download Resume</a>
            
        </div>    
    </div>

    <div class="contact-form">
        
        <form>
            <input type="text" placeholder="Name" />
            <input type="email" placeholder="Email" />
            <textarea placeholder="Message"></textarea>
            <button @click="sendMsg()">Send</button>
        </form>
    </div>

    

  </div>

</template>

<script>
export default {
    data() {
    return {
      activeTab: 'skills'
    };
  },
  methods: {
    goTo(id) {
      const element = document.getElementById(id);
      element.scrollIntoView({ behavior: "smooth" }, 10);
    },

    sendMsg() {
      console.log("send");
    }
    
    
  }
  

  
};
</script>
