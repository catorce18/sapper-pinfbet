<script>
	export let segment;
</script>

<nav class="navbar is-link is-spaced has-shadow" role="navigation" aria-label="main navigation">
	<div class="container">
  <div class="navbar-brand">
    <a class="navbar-item" href="/home">
      imagen
    </a>

    <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="actualNavbar">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a>
  </div>

  <div id="actualNavbar" class="navbar-menu">
    <div class="navbar-start">
      <a class="navbar-item" aria-current="{segment === 'home' ? 'page' : undefined}" href='/home'>
        Inicio
      </a>

      <a class="navbar-item" aria-current="{segment === 'about' ? 'page' : undefined}" href='/about'>
        Actividad
      </a>

      <div class="navbar-item has-dropdown is-hoverable">
        <a class="navbar-link" aria-current="{segment === 'perfil' ? 'page' : undefined}">
          Perfil
        </a>

        <div class="navbar-dropdown">
          <a class="navbar-item">
            Amigos
          </a>
					<hr class="navbar-divider">
          <a class="navbar-item">
            Cerrar sesion
          </a>
        </div>
      </div>
    </div>

    <div class="navbar-end">
      <div class="navbar-item">
        <div class="buttons">
          <a class="button is-primary">
            <strong>Sign up</strong>
          </a>
          <a class="button is-light">
            Log in
          </a>
        </div>
      </div>
    </div>
  </div>
	</div>
</nav>
