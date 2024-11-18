# go-cache-project

Este es un proyecto en Go que implementa una solución de caché sencilla para almacenar datos en memoria de manera eficiente. Utiliza la biblioteca `go-cache` para gestionar el almacenamiento temporal de claves y valores, ofreciendo una forma rápida de almacenar y recuperar información sin depender de una base de datos persistente.

## 🚀 Características

- Almacenamiento en memoria basado en claves.
- Soporte para expiración de entradas en la caché.
- Fácil integración en proyectos Go.
- Ideal para casos donde se requiera almacenamiento temporal rápido y sin persistencia.

## 📋 Requisitos

- Go 1.18 o superior.
- Conexión a Internet para instalar las dependencias.

## 📦 Instalación

1. Clona el repositorio:
   
   ```bash
   git clone https://github.com/langermanaxel/go-cache-project.git

2. Accede al directorio del proyecto:

   ```bash
   cd go-cache-project

3. Instala las dependencias necesarias:

   ```bash
   go mod tidy

## 🛠️ Uso
A continuación, se presenta un ejemplo de cómo utilizar este proyecto en un entorno local:
package main

import (
    "fmt"
    "time"
    "github.com/patrickmn/go-cache"
)

func main() {
    // Crear una nueva caché con un tiempo de expiración de 5 minutos y purga cada 10 minutos
    c := cache.New(5*time.Minute, 10*time.Minute)

    // Establecer un valor en la caché
    c.Set("clave", "valor", cache.DefaultExpiration)

    // Recuperar un valor de la caché
    valor, encontrado := c.Get("clave")
    if encontrado {
        fmt.Println("Valor encontrado:", valor)
    } else {
        fmt.Println("Valor no encontrado")
    }

    // Eliminar un valor de la caché
    c.Delete("clave")
}

## 
Aquí tienes el contenido en formato README listo para ser utilizado:

markdown
Copiar código
# go-cache-project

Este es un proyecto en Go que implementa una solución de caché sencilla para almacenar datos en memoria de manera eficiente. Utiliza la biblioteca `go-cache` para gestionar el almacenamiento temporal de claves y valores, ofreciendo una forma rápida de almacenar y recuperar información sin depender de una base de datos persistente.

## 🚀 Características

- Almacenamiento en memoria basado en claves.
- Soporte para expiración de entradas en la caché.
- Fácil integración en proyectos Go.
- Ideal para casos donde se requiera almacenamiento temporal rápido y sin persistencia.

## 📋 Requisitos

- Go 1.18 o superior.
- Conexión a Internet para instalar las dependencias.

## 📦 Instalación

1. Clona el repositorio:
   
   ```bash
   git clone https://github.com/langermanaxel/go-cache-project.git
Accede al directorio del proyecto:

bash
Copiar código
cd go-cache-project
Instala las dependencias necesarias:

bash
Copiar código
go mod tidy
🛠️ Uso
A continuación, se presenta un ejemplo de cómo utilizar este proyecto en un entorno local:

go
Copiar código
package main

import (
    "fmt"
    "time"
    "github.com/patrickmn/go-cache"
)

func main() {
    // Crear una nueva caché con un tiempo de expiración de 5 minutos y purga cada 10 minutos
    c := cache.New(5*time.Minute, 10*time.Minute)

    // Establecer un valor en la caché
    c.Set("clave", "valor", cache.DefaultExpiration)

    // Recuperar un valor de la caché
    valor, encontrado := c.Get("clave")
    if encontrado {
        fmt.Println("Valor encontrado:", valor)
    } else {
        fmt.Println("Valor no encontrado")
    }

    // Eliminar un valor de la caché
    c.Delete("clave")
}

## 📚 Documentación
Puedes encontrar más información sobre la biblioteca go-cache utilizada en este proyecto en la documentación oficial.

## 🤝 Contribuir
Si deseas contribuir a este proyecto, sigue estos pasos:

Realiza un fork del repositorio.
Crea una nueva rama (git checkout -b feature/nueva-funcionalidad).
Realiza tus cambios y confirma los commits (git commit -am 'Agregar nueva funcionalidad').
Empuja la rama (git push origin feature/nueva-funcionalidad).
Crea un Pull Request.

## 📧 Contacto
Si tienes preguntas o sugerencias, no dudes en contactarme:

Autor: Axel Langerman
GitHub: langermanaxel
Correo: axellangerman@yahoo.com
