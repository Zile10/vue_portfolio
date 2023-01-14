<template>
  <div id="testimonials">
    <div class="section-overlay">
      <h2 data-aos="zoom-in">Testimonials</h2>
      <div class="container">
        <div class="grid-div overflow-hidden">
  
          <!-- <TestimonialVue imgSrc="www.image.com"/> -->
  
          <TestimonialVue v-for="testimonial in testimonials" :key="testimonial"
            :imgSrc="testimonial.imgSrc"
            :name="testimonial.name"
            :surname="testimonial.surname"
            :quote="testimonial.quote"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TestimonialVue from '@/components/TestimonialVue.vue';
export default {
  name: 'HomeView',
  components: {
    TestimonialVue
  },
  data() {
    return {
      testimonials: [
        {
          imgSrc:"https://i.postimg.cc/3R126B29/Mkhuseli.jpg",
          name:"Mkhuseli",
          surname:"Mkeyiya",
          quote:"'I feel like I have known John for many years, he always puts the time to his work which is what puts him ahead of the class. He is always willing to assist where he can and he does it respectfully I wish him the best of luck in his future endeavours.'",
        },
        {
          imgSrc:"https://i.postimg.cc/4NqVrnhC/tyvon.jpg",
          name:"Tyvon",
          surname:"April",
          quote:"'John-Bruce Noad is a very professional person when it comes to his work. He is able to think of a design of a website and implement it in his Project. He has full understanding of what he is doing and is a very reliable person. I enjoyed working with him.'",
        },
        {
          imgSrc:"https://i.postimg.cc/635N8tzL/matthew-cropped.jpg",
          name:"Matthew",
          surname:"Thomas",
          quote:"'John is well-versed in his Development work. Alongside that, his ability to problem-solve his code is really amazing. Despite this, he is aware that he still has much more room for improvement. But overall as a Colleague who's seen his growth and as a developer, he takes time to help his fellow colleagues with their issues regarding code and considers it a learning curve to help with implementation of code error patches. He is driven and work consistently in all Front-End endeavors thus and always strives for Improvement.'",
        },

        {
          imgSrc:"https://i.postimg.cc/J46Pt1DK/Deno.jpg",
          name:"Deno",
          surname:"Rautenbach",
          quote:"'Weird. That's John. Don't get me wrong, the good kind of weird. It's always lively when he's present as his witty remarks often make me laugh like a Hyena. John is always busy helping someone in need whenever he can, further showing the depth of his wondrous intellect  and personality. Logical in his approach to everything, we vibrate on the same level in that sense, and for that I have a deep respect for John.'",
        },
        {
          imgSrc:"https://i.postimg.cc/MG8QkzV3/profile-1.jpg",
          name:"Camryn",
          surname:"Herandien",
          quote:"John-Bruce Noad is somebody  that is vital to any team, not only is he a point of reference when needed,  He is always there to help you. With him on your team makes tasks a whole lot easier and less stressful. I highly admire his work ethic and passion. 10*",
        },
        {
          imgSrc:"https://i.postimg.cc/T3h9Mgd5/t0.jpg",
          name:"Imraan",
          surname:"Bernken",
          quote:"John is a genius by heart, hard-working, constantly wants to improve and be better at everything he does. He is a very friendly and does mind helping others in need. A passionate person and its always a pleasure to engage in conversion with him.",
        },
      ]
    }
  },
}
</script>


<style>
#testimonials{
  background: url(https://i.postimg.cc/jSWj419b/alesia-unsplash-workplace.jpg);
}
.grid-div {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}
.grid-div > * {
  grid-column: span 1;
  width: 90%;
  margin: auto;
}

div.scroll {
  height: 200px;
}
.scroll {
  overflow-y: hidden;
  -webkit-mask-image: linear-gradient(to bottom, black 75%, transparent 100%);
  mask-image: linear-gradient(to bottom, black 75%, transparent 100%);
}
.scroll::-webkit-scrollbar {
  width: 10px;
}
.scroll::-webkit-scrollbar-track {
  background-color: #fff;
  border-radius: 50px;
}
.scroll::-webkit-scrollbar-thumb {
  background-image: var(--primaryLinearGradient);
  border-radius: 50px;
}
.scroll:hover {
  overflow-y: auto;
}
.testimonial-card .btn {
  margin-top: 10px;
  background-color: var(--secondaryColor);
  border-color: var(--secondaryColor);
}
.testimonial-card .btn:hover {
  background-image: var(--primaryLinearGradient);
  border-color: var(--secondaryColor);
  scale: 1.05;
}

@media only screen and (max-width: 900px) {
  .grid-div {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
  }
}
@media only screen and (max-width: 500px) {
  .grid-div {
    display: grid;
    grid-template-columns: repeat(1, 1fr);
  }
}
</style>