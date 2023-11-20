<script setup>
import ProjectCard from './ProjectCard.vue'

// const project1 = {
//     title : 'Md Nazmul Huda',
//     description : 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius at enim eum illum aperiam placeat esse? Mollitia omnis minima saepe recusandae libero, iste ad asperiores! Explicabo commodi quo itaque! Ipsam!',
//     image:'https://images.unsplash.com/photo-1573133111521-7c60dc32bb9c?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D'
// }

// const project2 = {
//     title : 'Md Saiful Islam',
//     description : 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius at enim eum illum aperiam placeat esse? Mollitia omnis minima saepe recusandae libero, iste ad asperiores! Explicabo commodi quo itaque! Ipsam!',
//     image:'https://plus.unsplash.com/premium_photo-1699533134796-d26b303153c4?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D'
// }

const projects = [
    {
    title : 'Title 1',
    description : 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius at enim eum illum aperiam placeat esse? Mollitia omnis minima saepe recusandae libero, iste ad asperiores! Explicabo commodi quo itaque! Ipsam!',
    image:'https://plus.unsplash.com/premium_photo-1699533134796-d26b303153c4?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D'

    },
    {
    title : 'Title 2',
    description : 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius at enim eum illum aperiam placeat esse? Mollitia omnis minima saepe recusandae libero, iste ad asperiores! Explicabo commodi quo itaque! Ipsam!',
    image:'https://images.unsplash.com/photo-1573133111521-7c60dc32bb9c?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D'
}
]
</script>

<template>
    <!-- Projects Section-->
    <section class="py-5" id="features">
                <div class="container px-5 mb-5">
                    <div class="text-center mb-5">
                        <h1 class="display-5 fw-bolder mb-0"><span class="text-gradient d-inline"> Features </span></h1>
                    </div>
                    <div class="row gx-5 justify-content-center">
                        <div class="col-lg-11 col-xl-9 col-xxl-8">

                            <!-- {{ projects }} -->
                           
                            <!-- Project Card 1-->
                           <!-- <ProjectCard :title="project1.title" :description="project1.description" :image="project1.image"></ProjectCard>
                           <ProjectCard :title="project2.title" :description="project2.description" :image="project2.image"></ProjectCard> -->

                           <!-- using loop -->

                           <ProjectCard
                           v-for="project in projects"
                            :title="project.title"
                             :description="project.description"
                              :image="project.image"></ProjectCard> 
                        </div>
                    </div>
                </div>
            </section>
            <!-- Call to action section-->
            <section class="py-5 bg-gradient-primary-to-secondary text-white" id="contact">
                <div class="container px-5 my-5">
                    <div class="text-center">
                        <h2 class="display-4 fw-bolder mb-4"> Call-to-Action </h2>
                        <a class="btn btn-outline-light btn-lg px-5 py-3 fs-6 fw-bolder" href="#">
                                <i class="bi bi-whatsapp"></i>
                                 01845076221 
                            </a>
                    </div>
                </div>
            </section>
</template>