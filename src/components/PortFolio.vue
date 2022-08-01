<template>

<div style="background-color:white;">
 <h4>Sample projects</h4>
  <hr class="border-grey-light border-t">
 <div class="p-10 grid grid-cols-1 sm:grid-cols-3 md:grid-cols-3 lg:grid-cols-3 xl:grid-cols-3 gap-5">
    <!--Card 1-->
        <div v-for="project in projects" :key="project.id">
       
    <div class="rounded overflow-hidden shadow-lg">
      <img class="w-full hover:scale-75 ease-in duration-500"  src="https://images.unsplash.com/photo-1471879832106-c7ab9e0cee23?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxleHBsb3JlLWZlZWR8Mnx8fGVufDB8fHx8&auto=format&fit=crop&w=500&q=60" alt="Mountain">
      <div class="px-8 py-4">
        <div class="font-bold text-xl mb-2">Mountain</div>
        <p class="text-gray-700 text-base">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, Nonea! Maiores et perferendis eaque, exercitationem praesentium nihil.
        </p>
      </div>
   <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 border border-blue-700 rounded">
  View in Github
</button><br>
    </div>
    </div>
  </div>
  
</div>

</template>
<script>
import portfolio from "./portfolio.json";
export default {
    name: "PortFolio",
    data() {
        return {
          projects: portfolio,
        }
    }
}
</script>
<style>
.zoom-image:hover .zoom-image {
  @apply scale-150;
}
.zoom-image:hover .zoom-text {
  @apply scale-100;
}
</style>