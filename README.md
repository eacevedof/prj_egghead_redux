# prj_egghead_redux
https://egghead.io/courses/getting-started-with-redux

<h1>
    <a href="https://egghead.io/courses/getting-started-with-redux">
        courses/getting-started-with-redux
    </a>
</h1>

<h2>
    <a href="https://egghead.io/lessons/javascript-redux-the-single-immutable-state-tree">
        1. lessons/javascript-redux-the-single-immutable-state-tree
    </a>
</h2>
<ol>
    <li>
        El objeto global <b>state</b>. Controla el último estado, cambio realizado en la app.
        Es la mínima representación de los datos en la aplicación.
    </li>
    <li>
        Admite cualquier tipo de variable.
    </li>
    <li>
        Puede ser entero para un simple contador o un objeto complejo.
    </li>
    <li>
        Se actualiza al ejecutar un evento. 
    </li>
    <li>
        Por ejemplo, si tenemos un modelo Notas. <br/>
        con las propiedades: id, activa, completada pasaría a guardarse en el estado 
        como un objeto con una propiedad de tipo array notas y en esta se apliaría cada registro
        de la tabla Notas. 
        Cada registro sería un objeto "Nota" del tipo: {id:,completed:,text:}
    </li>
</ol>

<hr/>
<h2>
    <a href="https://egghead.io/lessons/javascript-redux-describing-state-changes-with-actions">
        2. lessons/javascript-redux-describing-state-changes-with-actions
    </a>
</h2>
<ol>
    <li>
        El estado es de tipo readonly. No se puede forzar una asignación o un borrado directamente por código
        Es la mínima representación del cambio realizado sobre los datos.
    </li>
    <li>Para modificar el estado, se debe hacer por medio de una <b>action</b></li>
    <li>
        La variable acción, es una variable de tipo objeto y debe tener una propiedad
        <b>type</b> de tipo string preferiblemente. <br/>
        Ejemplo: {type: "INCRMENT"}
    </li>
    <li>
        Nota: Si estamos en un formulario con varios botones asociariamos a cada evento de esos botones
        con acciones.  Entonces si tenemos un botón guardar deberiamos definir una accion {type:"GUARDAR"}
        <br/><br/>
        Supongamos que tenemos varios objetos (notas). Si deseamos añadir un nuevo objeto dinámicamente a cada 
        uno de ellos le asignaremos una propiedad <b>index</b> esto nos permitirá tener localizado el objeto
        de forma atómica.
        <br/><br/>
        Ejemplos acciones: 
            action: {id: 0,text:"Nota Uno",type:"ADD_NOTA"}<br/>
            action: {filter: "SHOW_ACTIVE",type:"SET_VISIBILITY_FILTER"}<br/>
            action: {filter: "SHOW_COMPLETED",type:"SET_VISIBILITY_FILTER"}<br/>
    </li>
    <li>
        En conclusión, solo se puede tocar el estado por medio de la ejecución de acciones.
        Estas acciones a groso modo son eventos lanzados por el usuario o por una conexión en red.
    </li>
</ol>

<hr/>
<h2>
    <a href="https://egghead.io/lessons/javascript-redux-pure-and-impure-functions">
        3. lessons/javascript-redux-pure-and-impure-functions
    </a>
</h2>
<ol>
    <li>Funciones puras: Dependen solo de los valores de los argumentos</li>
    <li>No modifican sus argumentos</li>
    <li>
        Funciones impuras, hacen llamadas a bd, cambian valores de sus variables o variables globales,
        enviar datos a la pantalla o guardar en un archivo (a esto se llama efecto secundario).
        Estas acciones hacen que el programa sea más dificil de predecir.<br/>
        La programación funcional (funciones puras) intenta minimizar esta caracteristica.
    </li>
    <li>
        Muchas de las funciones que se tienen que escribir en Redux deben ser puras.
    </li>
</ol>

<hr/>
<h2>
    <a href=" ">
        4. 
    </a>
</h2>
<ol>
    <li>
    </li>
    <li>
    </li>
    <li>
    </li>  
</ol>

<hr/>
<h2>
    <a href=" ">
        5.
    </a>
</h2>
<ol>
    <li>
    </li>
    <li>
    </li>
    <li>
    </li>  
</ol>