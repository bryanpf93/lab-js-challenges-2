1. Challenge 1:
  - Answer:  b
  - Explanation: La variable foo esta definida en el scope global con el valor "abc". La función bar() modifica directamente esa variable global (no crea una nueva). El console.log dentro de la función imprime "xyz" y el console.log exterior también muestra "xyz" porque la variable global fue actualizada.
    


2. Challenge 2:
  - Answer: c
  - Explanation: La variable a esta definida en el scope global con el valor 1. El parámetro a de la función example(a) crea una nueva variable local que oculta (shadowing) la variable global. Cuando se llama a la función, el valor 1 se pasa por valor al parámetro local. Dentro de la función se cambia a 10, pero este cambio solo afecta a la variable local. Por lo tanto, el console.log dentro de la funcion valdra 10 y el console.log de fuera valdra 1


3. Challenge 3:
  - Answer: c
  - Explanation: Las declaracionees de funcion se elevan (hoisting) al inicio del contexto, por eso puedes invocarla antes de declararla


4. Challenge 4:
  - Answer: c
  - Explanation: b no es una copia del objeto a, sino una referencia al mismo objeto en memoria. Cuando se modifica b.num = 90, tambien se modifica a.num porque ambas variables apuntan al mismo objeto. En js los objetos pasan y asignan por referencia


5. Bonus - Challenge 5:
  - Answer: c
  - Explanation:
  . La función recibe una referencia al objeto rabbit1.
  . obj.age = 10 modifica el objeto original.
  . obj = { name: "Ada", age: 20 } crea un objeto nuevo y solo cambia la variable local.
  . El objeto original sigue siendo el mismo.
  . La función devuelve el nuevo objeto.
    rabbit1 → { name: "Bob", age: 10 }
    rabbit2 → { name: "Ada", age: 20 }
