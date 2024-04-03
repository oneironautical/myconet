<script lang='ts'>
    import svelteLogo from '../assets/svelte.svg'
    import Counter from '../components/Counter.svelte'
    import WeatherForecast from '../components/WeatherForecast.svelte';
    import { Link } from 'svelte-routing';
    import AuthorizeView from '../AuthorizeView.svelte';
    import Logout from '../components/Logout.svelte';
    
    </script>

<div id='navbar'>
  <div id='test'>Ya Boi</div>
  <div id='navbar-background'></div>
  
 </div>

<main>
  <div id='contain'>
    <div class="card">
  
      <WeatherForecast/>
    </div>
     <div class="card">
       <WeatherForecast/>
     </div>
    <div class="card">
      <WeatherForecast/>
      </div>
      <div class="card">
        <WeatherForecast/>
      </div>
    </div>
</main>

<style>

 #contain{
  margin-top: 10vh; 
 }
  #test{
  z-index: 1;
  }
  #navbar {
  width: 100%;
  height: 10vh;
  position: fixed;
  top: 0;
  color: white;
  text-align: center;
  vertical-align: middle;
  line-height: 90px;
  border-top: 1px solid black;
  border-bottom: 1px solid black;
  background-color: #242424;
  }

  #navbar-background {
  background-image: url("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRd37BWRvqIAkWiN6vbz5qSVKsYzdZw0ilvLMF7yOPM9g&s");
  opacity: 0.2;
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 10vh;
  z-index: .01;
  }


</style>

    <!--<AuthorizeView let:user_identity_email>
    <main>
        <div>
          <a href="https://svelte.dev" target="_blank" rel="noreferrer">
            <img src={svelteLogo} class="logo svelte" alt="Svelte Logo" />
          </a>
        </div>
        <h1>Svelte Demo</h1>
        <Logout>Log Out {user_identity_email}</Logout> |
        <Link to="/register">Register</Link>
        <div class="card">
          <Counter />
          <WeatherForecast/>
        </div>
      </main>
      
      
      <style>
        .logo {
          height: 6em;
          padding: 1.5em;
          will-change: filter;
          transition: filter 300ms;
        }
        .logo:hover {
          filter: drop-shadow(0 0 2em #646cffaa);
        }
        .logo.svelte:hover {
          filter: drop-shadow(0 0 2em #ff3e00aa);
        }
        
      </style>
    </AuthorizeView>-->