<script setup>
defineProps({
  title: '',
  description: '',
  image: ''
})
</script>

<template>
     <div class="card overflow-hidden shadow rounded-4 border-0 mb-5">
                                <div class="card-body p-0">
                                    <div class="d-flex align-items-center">
                                        <div class="p-5">
                                            <h2 class="fw-bolder"> {{ title }} </h2>
                                            <p>{{ description }}</p>
                                        </div>
                                        <img class="img-fluid" :src="image" alt="..." style="width: 300px;height: 400px;"/>
                                    </div>
                                </div>
                            </div>
                            
</template>