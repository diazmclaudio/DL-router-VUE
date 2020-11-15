<template>
  <div>
    <nav class="navbar navbar-dark bg-dark navbar-expand-lg fixed-top" id="mainNav">
        <div class="container"><router-link class="navbar-brand" :to="{name:'Portada'}">V8</router-link><button data-toggle="collapse" data-target="#navbarResponsive" class="navbar-toggler" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation"><i class="fa fa-bars"></i></button>
            <div
                class="collapse navbar-collapse" id="navbarResponsive">
                <div class="navbar-nav ml-auto">
                      <router-link class="nav-link" :to="{name:'Portada'}">Portada</router-link>
                      <router-link class="nav-link" :to="{name:'SobreMi'}">Sobre mi</router-link>
                      <router-link class="nav-link" to="/contacto">Contacto</router-link>
                      <router-link class="nav-link" to="/post/1">Blog</router-link>
                </div>
            </div>
        </div>
    </nav>
    <router-view></router-view>
  </div>
  
</template>

<script>
export default {
  name: 'App'
}
</script>

<style scoped>

#menu-v8 a{
  text-shadow: 1px 1px #000;
}
</style>