<script>
  import { goto } from '@sapper/app';
   export let segment;
   export async function preload(page, session)
   {

   }
   function handleEdit()
   {
     goto('/editar');
   }
</script>



<div class="container">
<div class="columns pt-5">
  <div class="column is-1 ">
    <figure class="image is-128x128 ">
    <img src="lagarto.jpeg" class="is-rounded" alt="foto de perfil">
    </figure>
  </div>
  <div class="column is-half pl-6">
    <h1 class="is-size-3 has-text-weight-bold">Nombredeusuario</h1>
    <form on:submit|preventDefault={handleEdit} name="editar" class="box">
    <div class="control">
        <button class="button is-danger" type="submit">
          Editar Perfil
        </button>
    </div>
    </form>
    <div class="columns has-text-centered">
      <div class="column is-2">
        <p>Mates</p>
        <p class="is-size-3">8</p>
      </div>
      <div class="column is-2">
        <p>Mates</p>
        <p class="is-size-3">8</p>
      </div>
      <div class="column is-2">
        <p>Mates</p>
        <p class="is-size-3">8</p>
      </div>
      <div class="column is-2">
        <p>Mates</p>
        <p class="is-size-3">8</p>
      </div>

    </div>
  </div>

</div>
<hr class="mt-0">
</div>



<nav class="navbar is-white is-spaced " role="navigation" aria-label="main navigation">
	<div class="container">
  <div class="navbar-brand">


    <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="actualNavbar">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a>
  </div>

  <div id="actualNavbar" class="navbar-menu">
    <div class="navbar-start">
      <a class="navbar-item" aria-current="{segment === 'perfil' ? 'page' : undefined}" href='/perfil/datos'>
        Mis Datos

      </a>

      <a class="navbar-item" aria-current="{segment === 'perfil' ? 'page' : undefined}" href='/perfil/pinfcoins'>
        Pinfcoins
      </a>

      <div class="navbar-item has-dropdown is-hoverable">
        <a class="navbar-link" aria-current="{segment === 'perfil' ? 'page' : undefined}">
          Mis apuestas
        </a>

        <div class="navbar-dropdown">
          <a class="navbar-item" href='/perfil/apuestas'>
            General
          </a>
					<hr class="navbar-divider">
          <a class="navbar-item" href='/perfil/ganadas'>
            Apuestas ganadas
          </a>
					<hr class="navbar-divider">

        </div>
      </div>
    </div>

    <div class="navbar-end">
      <div class="navbar-item">
        <div class="buttons">

        </div>
      </div>
    </div>
  </div>
	</div>
</nav>
