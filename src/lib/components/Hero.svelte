<script lang="ts">
import Down from '../images/1492533501-arrow-30_83308.svg';
</script>

<div>
  <h1>Front End Developer</h1>
  <h2>Jenny Feragen</h2>
  <p>
    Scroll down to learn more <br>
    <img src={Down} alt="down arrow">
  </p>
</div>

<style lang="scss">
  div {
      color: var(--primary);
      min-height: 100vh;
      text-align: center;
      display: flex; 
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }

    h1 {
      font-size: var(--font-size-xxxl);
      margin: var(--spacing-null);
    }

    h2 {
      font-size: var(--font-size-xl);
    }

    p{
      font-style: italic;
    }

    img {
      width: 50px;
      height: 50px;
      animation: 2s linear infinite 0s bounce;
    }

    @keyframes bounce {
    from {
      /* pushes the sun down past the viewport */
      transform: translateY(1vh);
    }
    to {
      /* returns the sun to its default position */
      transform: translateY(5vh);
    }
  }

  @media only screen and (max-width: 600px){
    div {
      min-height: 100vh;
    }

    h1 {
      font-size: var(--font-size-xxl);
    }

    h2 {
      font-style: var(--font-size-m);
    }
  }
</style>