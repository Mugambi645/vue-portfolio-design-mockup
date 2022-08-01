<template>
<div>

  <div class="resume bg-white shadow-lg p-8 md:p-16">

    <hr class="border-grey-light border-t">
    <main class="py-3">
      <section class="bio">
        <h2 class="flex items-center">
          <i class="em em-wave text-lg mr-2"></i>
          <span class="text-2xl font-semibold">Bio</span>
        </h2>
        <p class="text-gray-800">Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet mollitia distinctio sed dolore quibusdam est ad, voluptate aspernatur totam molestias alias voluptatem? Officia cum quia expedita dolore adipisci pariatur odio.</p>
      </section>
      <section class="experience">
        <h2 class="flex items-center">
          <i class="em em-computer text-lg mr-2"></i>
          <span class="text-2xl font-semibold">Experience</span>
        </h2>
        <p class="text-gray-800">Lorem ipsum dolor sit amet consectetur adipisicing elit. Excepturi quidem quis omnis quisquam dolor facere cum laborum dolores nesciunt magni eius, cumque reprehenderit modi sunt sed molestiae veritatis, atque eos?</p>
      </section>
      <section class="education">
        <h2 class="flex items-center">
          <i class="em em-mortar_board mr-2 text-lg"></i>
          <span class="font-semibold text-2xl">Education</span>
        </h2>
        <p class="text-gray-800">Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsum ab cupiditate accusamus ut veniam ea expedita modi rem sequi exercitationem cum eius tempora repellat provident numquam dolore, reprehenderit adipisci eos.</p>
      </section>
      <aside class="skills bg-gray-200 px-4 py-3 rounded-lg">
        <h2 class="uppercase tracking-widest text-base text-xl text-gray-600 font-semibold">Skills</h2>
        <ul class="">
          <li>
     <p><font-awesome-icon icon="fa-solid fa-circle-check" /> gdhjd</p>
          
            
          </li>
             <li>
     <p><font-awesome-icon icon="fa-solid fa-circle-check" /> gdhjd</p>
          
            
          </li>
             <li>
     <p><font-awesome-icon icon="fa-solid fa-circle-check" /> gdhjd</p>
          
            
          </li>
             <li>
     <p><font-awesome-icon icon="fa-solid fa-circle-check" /> gdhjd</p>
          
            
          </li>
             <li>
     <p><font-awesome-icon icon="fa-solid fa-circle-check" /> gdhjd</p>
          
            
          </li>
             <li>
     <p><font-awesome-icon icon="fa-solid fa-circle-check" /> gdhjd</p>
          
            
          </li>
             <li>
     <p><font-awesome-icon icon="fa-solid fa-circle-check" /> gdhjd</p>
          
            
          </li>
        </ul>
      </aside>
    </main>
    <hr class="border-grey-light border-t">

  </div>
</div>



</template>
<script>
export default {
    name: "ResumeComponent",
    data() {
        return {
            title: "Hello nav"
        }
    }
}
</script>
<style lang="scss">
.resume {
  flex-basis: 900px;
}

main {
  @media (min-width: 900px) {   
  display: grid;
  grid-template-areas:
    "skills bio bio"
    "skills experience experience"
    "skills education education";
  }
  grid-gap: 2rem;
  grid-template-columns: 1fr 1fr 1fr;
}

.bio {
  grid-area: bio;
}

.experience {
  grid-area: experience; 
}

.education {
  grid-area: education; 
}

.skills {
  grid-area: skills; 
}

</style>