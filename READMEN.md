# Saludos en GO

Este paquete proporciona una forma simple de obtener saludos personalizados en Go.

## Instalacion
Ejecutar el siguiente comando para instalar paquete:
```bash
go get -u github.com/MaximoPeter/greetings
```

## Uso
Aqui tienes un ejemplo de como utilizar el paquete en tu codigo:

```go
package main

import (
	"fmt"
	"github.com/MaximoPeter/greetings"
)

func main() {
	message, err := greetings.Hello("Peter")

	if err != nil {
		fmt.Println("Ocurrio un error:", err)
        return
	}

    fmt.Println(message)
}

```

Este ejemplo importa el paquete github.com/MaximoPeter/greetings y llama a la funcion Hello
saludo personalizado. Si ocurre un error, se imprime un mensaje de error.
