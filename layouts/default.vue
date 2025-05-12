<template>
  <div>
    <header>
      <nav>
        <ul>
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/services">Services</NuxtLink></li>
          <li><NuxtLink to="/contact">Contact</NuxtLink></li>
          </ul>
      </nav>
    </header>

    <Nuxt />

    <footer>
      <p>&copy; {{ new Date().getFullYear() }} Your Name/Practice Name. All rights reserved.</p>
    </footer>
  </div>
</template>

<style>
/* Basic styling for the layout */
body {
  font-family: sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f4f7f6; /* Use your calming colors */
  color: #333;
}

header {
  background-color: #a2d5cf; /* Use your calming colors */
  padding: 1rem 0;
  text-align: center;
}

nav ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

nav ul li {
  display: inline;
  margin: 0 15px;
}

/* Style NuxtLink components */
nav ul li a {
  text-decoration: none;
  color: #333;
  font-weight: bold;
}

/* Active link styling (optional) */
nav ul li a.nuxt-link-exact-active {
  color: #007bff; /* Or another highlight color */
}

footer {
  text-align: center;
  padding: 20px;
  background-color: #333; /* Darker color for footer */
  color: white;
}
</style>
