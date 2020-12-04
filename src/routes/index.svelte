<script>
  import { goto } from '@sapper/app';
  let em,pw;

  function handleLogin()
  {
    alert(em+pw);
    em='';
    pw='';
    goto('/home');
  }
</script>


<svelte:head>
	<title>PINFBet</title>
</svelte:head>


<body>
<div class="hero is-primary is-fullheight">
<div class="hero-body">
<div class="container has-text-centered">
  <h1 class="title has-text-centered is-size-3">Inicia sesion</h1>
  <div class="columns subtitle is-centered is-half pt-3">

    <form on:submit|preventDefault={handleLogin} name="login" class="box">
    <div class="field">
      <label class="label" for="email">email address</label>
      <div class="control has-icons-left">
        <input class="input" bind:value={em} type="email" autocomplete="email" name="email" placeholder="Correo electrónico">
        <span class="icon is-small is-left">
          <i class="fas fa-envelope"></i>
        </span>
      </div>
    </div>
    <div class="field">
      <label class="label" for="password">password</label>
      <div class="control has-icons-left">
        <input class="input" bind:value={pw} type="password" maxlength="25" name="password" placeholder="Contraseña">
        <span class="icon is-small is-left">
          <i class="fas fa-lock"></i>
        </span>
      </div>
    </div>
    <div class="field">
    <div class="control">
        <button class="button is-link" type="submit">
          Log in
        </button>
    </div>
    </div>
    </form>
  </div>
</div>
</div>
<p><strong>Try editing this file (src/routes/index.svelte) to test live reloading.</strong></p>
</div>
</body>
