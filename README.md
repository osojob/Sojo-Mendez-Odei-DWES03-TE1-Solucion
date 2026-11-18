# 📘 DWES03 - Tarea de Evaluación [1/2]

## 📝 Descripción general

El objetivo de esta tarea es que **diseñes un servicio web basado en una [API](https://es.wikipedia.org/wiki/API) REST, utilizando la arquitectura [MVC](https://es.wikipedia.org/wiki/Modelo%E2%80%93vista%E2%80%93controlador) y que permita realizar operaciones [CRUD](https://es.wikipedia.org/wiki/CRUD) desde un [cliente Rest](https://farwebs.es/programacion/que-es-rest-client/).**

La aplicación **no tendrá interfaz gráfica**: toda la comunicación entre el cliente y el servicio se realizará **mediante consultas HTTP e** intercambio de datos en formato JSON.

Este proyecto se desarrollará en dos tareas evaluativas:

- **TE1 – Diseño:** definirás la aplicación, sus datos, las operaciones que ofrecerá y su arquitectura.

- **TE2 – Desarrollo:** programarás el servicio web a partir del diseño realizado y aprobado en esta primera tarea.

> [!IMPORTANT]
> 
> Antes de empezar a diseñar, te recomiendo leer el enunciado de la TE2 para que conozcas los requisitos que tiene que tener el sistema.

---

## 🎯Objetivo de la Tarea

En esta primera parte del proyecto deberás diseñar un servicio web que permita gestionar información mediante operaciones REST. Para ello, **definirás las operaciones disponibles, los datos que se van a gestionar, el flujo de llamadas para realizar una consulta, el formato de las respuestas respuestas y la arquitectura que seguirá la aplicación.**

##### Temática del Servicio:

Tienes libertad para elegir el tema de la aplicación. Pero, deberás tener en cuenta que la aplicación deberá cumplir con los siguientes requisitos: gestionar una entidad principal para permitir las operaciones CRUD, implementar persistencia de datos mediante ficheros CSV y permitir el intercambio de información entre el cliente y el servicio mediante JSON.

> [!TIP]
> 
> Puedes desarrollar or ejemplo un sistema de gestión, una tienda en línea, un sistema de reservas u otro servicio que te interese.
> 
> Asegúrate de elegir una temática que sea versátil, ya que **en futuras unidades didácticas seguirás ampliando las funcionalidades de esta aplicación.**

---

## 🎯 Objetivos de aprendizaje

- Planificar el diseño de un servicio web basado en una API REST.

- Definir las operaciones CRUD que ofrecerá el servicio, especificando los métodos HTTP y sus correspondientes endpoints.

- Identificar los datos que gestionará la aplicación y cómo se almacenarán mediante ficheros CSV.

- Diseñar la arquitectura del servicio siguiendo el patrón MVC, identificando sus principales componentes y responsabilidades.

- Representar el flujo de comunicación entre el cliente REST y el servicio web, incluyendo las peticiones HTTP y las respuestas en formato JSON.

---

## 🛠️ Ejercicios

#### Ejercicio 1: Descripción del Proyecto

- Describe de manera detallada el **nombre y temática del servicio**

- **Define la entidad principal**que gestionará el servicio y **enumera los campos** que tendrá cada registro.

> [!NOTE]
> 
> Ejemplo: si tu aplicación consiste en un servicio de gestión de *ideas* un registro podría tener la siguiente estructura:
> 
> | Campo         | Descripción                         |
> | ------------- | ----------------------------------- |
> | `id`          | Identificador único de la nota.     |
> | `autor`       | Autor de la nota.                   |
> | `titulo`      | Título de la nota.                  |
> | `descripcion` | Contenido o descripción de la nota. |
> | `fecha`       | Fecha de creación de la nota.       |

- **Describe brevemente en qué consisten los cinco tipos de consulta** que se van a poder realizar en tu servicio:
  
  - `GET All` y `GET byID`
  
  - `POST`
  
  - `PUT`
  
  - `DELETE`

#### Ejercicio 2: Diagrama de arquitectura y flujo de funcionamiento

Utilizando una herramienta digital, **representa en un diagrama la arquitectura de tu servicio web y el flujo de llamadas para una consulta de tipo GETbyID y otra de tipo PUT**

Describe el flujo de llamadas **desde que el cliente realiza la consulta hasta que recibe una respuesta.**

El diagrama debe **mostrar los principales componentes de la aplicación**, cómo se relacionan entre sí y qué responsabilidades tiene cada uno. 

En el diagrama **deberán aparecer, como mínimo, los siguientes elementos:**

- **Cliente**

- **Front Controller**: punto de entrada de las peticiones al servicio.

- **Router y rutas**: cómo se identifica la operación que debe ejecutarse.

- **Controlador**: responsable de gestionar las operaciones .

- **DataHandler:** accede a los registros de datos.

- **Persistencia**: fichero CSV donde se almacenan los registros.

- **Respuesta de la API:** prepara y devuelve la respuesta al cliente.

> [!NOTE]
> 
> En el directorio de *recursos* podras encontrar: un [ejemplo](./recursos/Diagrama.png) de diagrama para una consulta POST *guardar idea* diseñado con *[draw.io](https://www.drawio.com/)*
