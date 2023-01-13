<template>
  <div id="contact">
    <div class="section-overlay">
      <h2 data-aos="zoom-in">Contact</h2>
      <div class="container mb-5">
        <form action="https://formspree.io/f/xqkjbnkv"  method="POST" target="_blank" name="myForm">
          <div data-aos="fade-right">
            <label for="#firstname" class="d-block">Name</label>
            <input id="firstname" name="firstName" type="text" placeholder="Enter your name" required>
          </div>
          <div data-aos="fade-left">
            <label for="#surname" class="d-block">Surname</label>
            <input id="surname" name="surname" type="text" placeholder="Enter your surname" required>
          </div>
          <div data-aos="fade-right">
            <label for="#email" class="d-block">Email Address</label>
            <input id="email" name="email" type="email" placeholder="Enter your email address" required>
          </div>
          <div data-aos="fade-left">
            <label for="#message" class="d-block" aria-placeholder="#contact">Message</label>
            <textarea id="message" name="message" cols="30" rows="10"></textarea>
          </div>
          <div data-aos="fade-right">
            <input id="submit" type="submit" value="submit" class="bevel2">
          </div>
        </form>    
      </div>
    </div>

  </div>
</template>

<script>

export default {
  name: 'HomeView',
  components: {

  },
  methods: {
    // validateForm() {     
    //   let x = document.forms["myForm"]
    //   x.forEach(item => {
    //     let y = item.value;
    //     if (y == "") {
    //       alert("Name must be filled out");
    //       return false;
    //     }
    //   });
    // }

  },
  data() {
    return {

    }
  },
}
</script>

<style>
input, textarea {
  width: 85%;
  color: #222;
  box-shadow: var(--primaryBoxShadow);
}

#submit {
  background-color: #333;
  text-transform: uppercase;
  cursor: pointer;
  color: white;
}
#submit:hover {
  border-color: var(--secondaryColor);
  scale: 1.02;
  background-image: var(--primaryLinearGradient);
  /* color: var(--secondaryColor); */
}
#submit:active {
  scale: 0.95;
}
</style>