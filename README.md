# Examen Técnico para Desarrollador Junior


## Parte 1: Preguntas Teóricas


### 1. Django


#### ¿Qué es Django y por qué se usa?

Django es un framework de código abierto hecho en Python que facilita el desarrollo rápido de aplicaciones web complejas, automatizando tareas repetitivas y pesadas, y permitiendo la reutilización de componentes en diferentes proyectos.




#### Explica brevemente el patrón MVC (Modelo-Vista-Controlador) y cómo se implementa en Django.

Django sigue el patrón MVC, que divide la aplicación en tres componentes:

- **Modelo**: Maneja la interacción con la base de datos y se encarga de los registros.
- **Vista**: Muestra esa información al usuario.
- **Controlador**: Gestiona las comunicaciones entre la vista y el modelo.

En Django:
- **Templates** funcionan como vistas.
- Las funciones del archivo `views.py` actúan como el *controlador*, utilizando las URLs de las vistas.
- **Modelos**: Se establecen en el archivo `models.py`, donde se definen los modelos que integran la aplicación.



#### ¿Qué es un modelo en Django y cómo se define?

El modelo representa la estructura de la base de datos en una aplicación Django. Se define mediante clases en el archivo `models.py`, donde cada clase representa una tabla y sus atributos son las columnas de esa tabla.


------------



### 2. Python


#### ¿Qué es un diccionario en Python y cómo se diferencia de una lista?

Un diccionario es una colección de datos que se encuentran agrupados por un par llave-valor, mientras que las listas son una agrupación de datos de diferente naturaleza, pero no tienen la estructura llave-valor.



#### Explica la diferencia entre `append()` y `extend()` en una lista de Python.

- **`append()`**: Permite agregar un solo elemento al final de la lista.
- **`extend()`**: Expande una lista ya existente con los elementos de una segunda lista, añadiendo esos elementos al final de la lista original.



#### ¿Qué es un decorador en Python? Proporciona un ejemplo simple.

Un decorador es una función que toma como parámetro una función y la modifica o extiende sin alterar su código original. Por ejemplo, un decorador que convierte un texto en mayúsculas:

    ```python

       def mayusculas(funcion_original):
            def envoltura():
            return funcion_original().upper()
        return envoltura

        @mayusculas
        def saludar():
            return "hola"

        print(saludar()) 

    ```  


------------



### 3. MySQL



#### ¿Qué es una base de datos relacional?

Es una estructura que organiza los datos mediante tablas, filas y columnas, permitiendo la creación de relaciones entre diferentes tablas. Evitando la duplicidad de datos y facilitando las consultas de los datos.



#### Explica la diferencia entre una clave primaria y una clave foránea.

La clave primaria es un identificador único que sirve para identificar cada registro y que no haya duplicados. La clave foránea por otro lado, es un campo en una tabla que apunta a la clave primaria de otra tabla, para así formar relaciones entre ellas.



#### ¿Cómo se realiza una consulta SELECT básica en MySQL?

*Para  columnas específicas:*
SELECT columna1,  columna2 FROM  nombre_tabla;


*Para todas las columnas:*
SELECT *FROM  nombre_tabla;




------------



### 4. API



#### ¿Qué es una API y para qué se utiliza?

Es una interfaz con reglas que permiten que diferentes aplicaciones se comuniquen entre sí, facilitando la integración y el uso de servicios externos.



#### Explica brevemente la diferencia entre una API REST y una API SOAP.

SOAP es un protocolo que dispone de funciones u operaciones. Está diseñado para exponer operaciones especificas mediante las funciones, solo transfiere datos XML. REST, en cambio, es un estilo de arquitectura que se basa en recursos y utiliza URL para acceder a ellos, permitiendo transferir datos en varios formatos, como JSON y HTML.



#### ¿Qué son los métodos HTTP comunes utilizados en una API REST?

*GET:* Recupera los datos que se encuentran en la URL.
*POST:* Envía los datos al servidor.
*PUT:* Se utiliza para actualizar los datos existentes en el servidor. 
*DELETE:* Se utiliza para eliminar el dato.



