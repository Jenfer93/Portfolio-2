<header>
  <nav>
    <ul>
      <li>
        <a class="button" href="#about">About</a>
      </li>
      <li>
        <a class="button" href="#contact">Contact</a>
      </li>
      <li >
        <a class="button" href="#myWork">My work</a>
      </li>
    </ul>
  </nav>
</header>

<style lang="scss">

header, nav, ul {
  margin: 0; 
  position: sticky;
  top: 0;
}

header {
  background-color: var(--dark-secondary);
  height: var(--spacing-xxl);
  display: flex;
  margin-bottom: var(--spacing-l);
}


nav {
  display: flex; 
  justify-content: flex-end;
  margin: auto;
  max-width: 1200px;
}

ul {
  display: flex; 
  margin-right: var(--spacing-m)
}
</style>