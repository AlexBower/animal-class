<template>
<div id="app">
  <div id="menu">
    <div id="title">
      <H1>Animal Class</H1>
    </div>
    <div id="nav">
      <div class="menu-item">
        <router-link to="/">
          <button>Name</button>
        </router-link>
      </div>
      <div class="menu-buffer"></div>
      <div class="menu-item">
        <router-link to="/gpa">
          <button>GPA</button>
        </router-link>
      </div>
      <div class="menu-buffer"></div>
      <div class="menu-item">
        <router-link to="/species">
          <button>Species</button>
        </router-link>
      </div>
    </div>
  </div>
  <router-view />
</div>
</template>

<style>
* {
  box-sizing: border-box;
}

body {
  margin: 50px 100px;
}

#menu {
  margin-bottom: 50px;
  display: flex;
  flex-direction: column;
  align-content: center;
  justify-content: center;
}

#title {
  display: flex;
  justify-content: center;
}

#nav {
  display: flex;
  justify-content: center;
}

.menu-item button {
  padding: 5px 15px;
  background-color: #8dc090;
  border-radius: 4px;
  border: solid black;
}

.menu-buffer {
  margin-left: 20px;
  margin-right: 20px;
}

#menu a {
  font-size: 30px;
  color: black;
  text-decoration: none;
}

</style>
