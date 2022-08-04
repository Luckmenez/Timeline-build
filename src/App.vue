<script setup>

</script>

<template>
  <section class="intro-text" >
    <div class="container">
        <h1>Tutorial Timeline</h1>
        <p>A timeline of my accomplishments.</p>
    </div>
  </section>
  <section class="timeline-section">
    <ul class="done-img">
      <li>
        <div>
          <time>2001</time> Lorem ipsum dolor sit amet consectetur adipisicing
            elit. Incidunt nostrum quidem eius repudiandae nam, nemo fuga
            architecto possimus id at rem beatae consequuntur dolor.
        </div>
      </li>
      <li>
        <div>
          <time>2002</time> Lorem ipsum dolor sit amet consectetur adipisicing
          elit. Incidunt nostrum quidem eius repudiandae nam, nemo fuga
          architecto possimus id at rem beatae consequuntur dolor commodi.
        </div> 
      </li>
      <li>
        <div>
          <time>2004</time> Lorem ipsum dolor sit amet consectetur adipisicing
          elit. Incidunt nostrum quidem eius repudiandae nam, nemo fuga
          architecto possimus id at rem beatae consequuntur dolor commodi.
        </div>
        </li>
        <li>
          <div>
            <time>2006</time> Lorem ipsum dolor sit amet consectetur adipisicing
            elit. Incidunt nostrum quidem eius repudiandae nam, nemo fuga
            architecto possimus id at rem beatae consequuntur dolor commodi.
          </div>
        </li>
        <li>
          <div>
            <time>2008</time> Lorem ipsum dolor sit amet consectetur adipisicing
            elit. Incidunt nostrum quidem eius repudiandae nam, nemo fuga
            architecto possimus id at rem beatae consequuntur dolor commodi.
          </div>
        </li>
    </ul>
  </section>
</template>

<style scoped>

.done-img {
  list-style-image: url('./assets/Google_Material_Design_check.svg.png');
}
.intro-text {
  background-color: var(--color-dark-grey);
  color: var(--white);
  padding: 2rem 0;
  font-size: 10px;
  font-family: 'Open Sans', sans-serif;
}

.container {
  margin: 0 auto;
  padding: 0 20px;
  text-align: center;  
}

.intro-text h1 {
  font-size: 2.5rem;
}

.timeline-section {
  width: 100%;
  overflow: hidden;
  font-size: 10px;
  font-family: 'Open Sans', sans-serif;
}

.timeline-section ul {
  background: white;
  padding: 5rem 0; 
}

.timeline-section ul li {
  list-style: none;
  position: relative;
  width: 5px; 
  margin: 0 auto; 
  padding-top: 5rem; 
  background: var(--color-blue);/** timeline color change */
}

.timeline-section ul li::after {
  content: "";
  position: absolute;
  left: 50%;
  bottom: 0;
  transform: translateX(-50%);
  width: 3rem;
  height: 3rem;
  border-radius: 50%;
  background: inherit;
}

.timeline-section ul li div {
  width: 40rem;
  font-size: 1.2rem;
  position: relative;
  bottom: 0;
  padding: 1.5rem;
  background: white;
  border-radius: 10px;
}

.timeline-section ul li div {
  top: 5.2rem;
  left: 45px;
}

.timeline-section ul li div::before {
  left: -15px;
  border-width: 8px 16px 8px 0;
  border-color: transparent var(--light-blue) transparent transparent;
}

time {
  display: block;
  font-size: 1.1rem;
  font-weight: 800;
  margin-bottom: 7px;
}

@media screen and (max-width: 600px) {
  .timeline-section ul li {
    margin-left: 2rem;
  }

  .timeline-section ul li div {
    width: calc(100vw - 91px);
  }

  .timeline-section ul li div {
    left: 45px;
  }

  .timeline-section ul li div::before {
    left: -15px;
    border-width: 8px 16px 8px 0;
    border-color: transparent var(--light-blue) transparent transparent;
  }
}
</style>