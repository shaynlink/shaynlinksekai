<template>
  <nav>
    <div>
      <router-link to="/" class="sekai_navbar_home">Shaynlink Sekai</router-link>
    </div>
    <div>
      <ul>
        <li><router-link to="/projects">projects</router-link></li>
        <li><router-link to="/blog">blog</router-link></li>
        <li><router-link to="/donate">donate</router-link></li>
        <li><router-link to="/projects"><button>github</button></router-link></li>
      </ul>
    </div>
  </nav>
</template>

<style lang="scss" scoped>
nav {
  display: flex;
  padding: 10px 50px;
  align-items: center;
  justify-content: space-between;
}

a {
  text-decoration: none;
  color: #fff;
}

ul {
  list-style: none; 
  display: flex;
  column-gap: 20px;
  align-items: center;
}

button {
  background: #39B15D;
  border-radius: 20px;
  padding: 9px 26px;
  border: none;
  color: #fff;
}

button:hover {
  cursor: pointer;
}

.sekai_navbar_home {
  font-weight: 700;
  font-size: 1.5rem;
}
</style>