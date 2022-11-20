<script>
  import svelteLogo from './assets/svelte.svg'
  import Counter from './lib/Counter.svelte'

  // Import the functions you need from the SDKs you need
  import { initializeApp } from "@firebase/app";
  import { getAnalytics } from "@firebase/analytics";
  // TODO: Add SDKs for Firebase products that you want to use
  // https://firebase.google.com/docs/web/setup#available-libraries

  // Your web app's Firebase configuration
  // For Firebase JS SDK v7.20.0 and later, measurementId is optional
  const firebaseConfig = {
    apiKey: "AIzaSyBeQH8fNooYXhvh6zjSOAKTaeoxN_fLpsw",
    authDomain: "archeryscoreapp.firebaseapp.com",
    projectId: "archeryscoreapp",
    storageBucket: "archeryscoreapp.appspot.com",
    messagingSenderId: "892363506674",
    appId: "1:892363506674:web:703a8ae3fdbad930f2216b",
    measurementId: "G-QRZ6ZNW12G"
  };

// Initialize Firebase
const app = initializeApp(firebaseConfig);
const analytics = getAnalytics(app);

  let score = 0
  const  add1 = () => {
    score += 1
  }

  const  add2 = () => {
    score += 2
  }

  const  add3 = () => {
    score += 3
  }

  const  add4 = () => {
    score += 4
  }

  const  add5 = () => {
    score += 5
  }

  const  add6 = () => {
    score += 6
  }

  const  add7 = () => {
    score += 7
  }

  const  add8 = () => {
    score += 8
  }

  const  add9 = () => {
    score += 9
  }

  const  add10 = () => {
    score += 10
  }

</script>

<main>
  <h1>Archery Score Counter</h1>
  <h2>Your Score: { score }</h2>
  <button on:click={add1} class="bw">
    1
  </button>
  <button on:click={add2} class="bw">
    2
  </button>
  <button on:click={add3} class="bb">
    3
  </button>
  <button on:click={add4} class="bb">
    4
  </button>
  <button on:click={add5} class="bl">
    5
  </button>
  <button on:click={add6} class="bl"> 
    6
  </button>
  <button on:click={add7} class="br">
    7
  </button>
  <button on:click={add8} class="br">
    8
  </button>
  <button on:click={add9} class="by">
    9
  </button>
  <button on:click={add10} class="by">
    10
  </button>
  
</main>

<style>
  .logo {
    height: 6em;
    padding: 1.5em;
    will-change: filter;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }
  .logo.svelte:hover {
    filter: drop-shadow(0 0 2em #ff3e00aa);
  }
  .read-the-docs {
    color: #888;
  }
</style>
