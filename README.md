# Juego número aleatorio.
## Python.

En primer lugar se creó un archivo .py (python), sobre el que se trabajó a través del programa visual studio code con la extensión de python.

A continuación, se analizará de forma breve el código utilizado:

Se encabezó el código con un **input random** que es nacesario para importar el módulo "random", utilizado para generar números aleatorios.

**def adivina_numero():** Define una función llamada adivina_numero.

**numero_secreto = random.randint(1, 100)** Genera un número aleatorio entre 1 y 100 y lo asigna a la variable numero_secreto.

**intentos = 0** Inicializa una variable llamada intentos a 0 para llevar la cuenta de cuántos intentos ha realizado el jugador.

   **print ("mensaje de bienvenida al jugador")** Los print son prompt, son mensajes que se envian al jugador. En el caso del juego crado se imprimieron       dos mensajes seguidos, uno de bienvenida y otro de intrucciones.

**while True:** Inicia un bucle infinito. El juego continuará hasta que el jugador adivine el número y rompa el bucle con la instrucción **break**

**guess = int(input("Introduce tu suposición: "))** Solicita al jugador que ingrese su suposición y la convierte a un entero.

**intentos += 1** Incrementa el contador de intentos en 1 cada vez que el jugador hace una suposición.

**if guess == numero_secreto:** Compara la suposición del jugador con el número secreto, indicando que si coinciden los números... 

  **print(f"¡Felicidades! Adivinaste el número en {intentos} intentos.")**   Imprime un mensaje de felicitaciones si el jugador adivina el número        muestra la cantidad de intentos.

**break:** Rompe el bucle, terminando el juego después de que el jugador adivina correctamente.

**elif guess < numero_secreto:** Si la suposición es menor que el número secreto, imprime un mensaje indicando que el número es más alto:

  **print("El número es más alto. Intenta de nuevo.")**: Imprime una pista    para que el jugador ajuste su siguiente suposición.

**else:** Si la suposición no es igual ni menor, significa que es mayor, por lo que imprime un mensaje indicando que el número es más bajo.

  **print("El número es más bajo. Intenta de nuevo.")** Imprime una   pista para que el jugador ajuste su siguiente suposición.

**if __name__ == "__main__"** Verifica si el script se está ejecutando como el programa principal.

**adivina_numero()** Llama a la función adivina_numero() para iniciar el juego cuando el script se ejecuta.
