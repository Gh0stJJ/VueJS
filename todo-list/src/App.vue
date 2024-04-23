<template>
  <nav id="navbar">
    <img src="./assets/logo.svg"  width="50"/>
    <div id="brand">
      Todo List App
    </div>

  </nav>

  <main class="container">
    <section>
      <form class="add-todo-form">
        <input type="text" placeholder="Todo Title" />
        <div>
          <button type="submit">Add Todo</button>
        </div>
      </form>
    </section>
    <section>
      <div id="todo">
        <p>Pasear al perro</p>
        <div>
          <!-- Caracter de x para cerrar -->
          <button id="remove-todo-btn">&times;</button> 
        </div>
      </div>
    </section>
  </main>
  
 
</template>



<script setup>

</script>


<!-- Add scoped to limit the styles to this component -->
<style scoped> 
#navbar{
  display: flex;
  
  align-items: center;
  background: var(--navbar-color);
  padding: 20px;
  margin-bottom: 30px;
  
}

#brand{
  font-size: 1.5rem;
  margin-left: 20px;
  color: var(--text-color);
}

.add-todo-form{
  display: flex;
  /* Uno a la izquierda y otro a la derecha */
  justify-content: space-between; 
  margin-top: 20px;
}

.add-todo-form input{
  padding: 10px;
  width: 80%;
  font-size: 1rem;
  border: solid 2px var(--border-color);
}

.add-todo-form button{
  padding: 10px 20px;
  font-size: 1rem;
  background: var(--border-color);
  color: var(--text-color);
  border: none;
  cursor: pointer;
  height: 50px;
}

#todo{
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: var(--border-color);
  margin-top: 30px;
  padding: 0 20px 0 20px;
  border-radius: 10px;
}

#remove-todo-btn{
  border: none;
  border-radius: 50%;
  cursor: pointer;
  height: 40px;
  width: 40px;
  font-size: 30px;
  background: var(--remove-btn-color);
  color: var(--text-color);
}

</style>
