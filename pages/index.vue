<template>
  <div class="container">
    
    <!-- <v-row>
      <v-col cols="12"> -->
      <div>
        <input v-model="idProducts" value="1">
        <button @click="onLoadProductStatic">Static</button>
        <button @click="onLoadProductDynamic">Dynamic</button>
      </div>
      
    <div>
      <Logo />
      <h1 class="title">
        cursoNuxt
      </h1>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          rel="noopener noreferrer"
          class="button--green"
        >
          Documentation
        </a>
        <a
          
          href="/products/"
          target="_blank"
          rel="noopener noreferrer"
          class="button--grey"
        >
          GitHub
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
data() {
  return {
    idProducts: ''
  }
},
methods: {
  onLoadProductStatic(){    
    this.$router.push('/products')
  },
  onLoadProductDynamic(){    
    this.$router.push('/products/' + this.idProducts)
  }  
}
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
