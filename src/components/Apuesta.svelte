<script>
  export let segment
  export let onClose
</script>

 
<div class="modal is-active">

  <div class="modal-background" > </div>
 
  <div class="modal-card">
 
    <header class="modal-card-head">
 
      <p class="modal-card-title">Apostar</p>
 
      <button on:click={onClose} class="delete" id="closetop" aria-label="close"></button>
 
    </header>
 
    <section class="modal-card-body">
      <div class="field">
        <div class="control">
          <label class="radio">
          <input type="radio" name="question">
          1 persona
          </label>
          <label class="radio">
          <input type="radio" name="question">
          2 personas
          </label>
        </div>
        </div>

      <div class="field">
        <label class="label">Elige</label>
        <div class="control has-icons-right">
          <input class="input" type="text" placeholder="Contrincante">
          <span class="icon is-small is-right">
          <i class="fas fa-user"></i>
          </span>
        </div>
        </div>

      <div class="field">
      <label class="label">vs.</label>
      <div class="control has-icons-right">
        <input class="input" type="text" placeholder="Contrincante">
        <span class="icon is-small is-right">
        <i class="fas fa-user"></i>
        </span>
      </div>
      </div>
        
        <div class="field">
        <label class="label">Convocatoria</label>
        <div class="control">
          <div class="select">
          <select>
            <option>-------</option>
            <option>Febrero</option>
            <option>Junio</option>
            <option>Septiembre</option>
          </select>
          </div>
        </div>
        </div>

        <div class="field">
          <label class="label">Asignatura</label>
          <div class="control">
            <div class="select">
            <select>
              <option>-------</option>
              <option>PINF</option>
              <option>AC</option>
              <option>SSI</option>
            </select>
            </div>
          </div>
          </div>
        
  
 
    </section>
 
    <footer class="modal-card-foot">
 
      <div class="field is-grouped">
        <div class="control">
          <button class="button is-link">Apostar</button>
        </div>
        <div class="control">
          <button class="button is-link is-light">Cancelar</button>
        </div>
        </div>
 
    </footer>
 
  </div>
 
  <!--<button on:click class="button is-danger is-large" aria-label="close" id="lanuchModal">Show Card Modal</button>-->
 
</div>

