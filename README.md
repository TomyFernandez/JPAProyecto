# JPAProyecto

![GitHub](https://img.shields.io/github/license/TomyFernandez/JPAProyecto)
![GitHub last commit](https://img.shields.io/github/last-commit/TomyFernandez/JPAProyecto)
![GitHub issues](https://img.shields.io/github/issues/TomyFernandez/JPAProyecto)

## Descripción

Este proyecto es una práctica de JPABase, con el objetivo de aprender a utilizar varias herramientas y tecnologías. Se han creado 2 artículos (carne y yogurt), un cliente con un domicilio, y una factura con 2 detalles de facturas, así como las categorías de los artículos.

## Tecnologías Utilizadas

- **H2**: Base de datos en memoria y en disco.
- **Hibernate**: ORM (Object-Relational Mapping) para Java.
- **Lombok**: Biblioteca para reducir el código boilerplate en Java.
- **Java**: Lenguaje de programación utilizado para el desarrollo del proyecto.

## Objetivo del Proyecto

El objetivo principal de este proyecto es aprender a utilizar las herramientas mencionadas anteriormente. Se ha logrado este objetivo mediante la creación de entidades, relaciones y la persistencia de datos en la base de datos H2.

## Características

- Creación de entidades: `Articulo`, `Categoria`, `Cliente`, `Domicilio`, `Factura`, `DetalleFactura`.
- Relaciones entre entidades: `OneToMany`, `ManyToMany`, `OneToOne`.
- Persistencia de datos en la base de datos H2.
- Uso de Lombok para reducir el código boilerplate.

## Instrucciones de Uso

1. **Clonar el Repositorio**:
   ```sh
   git clone https://github.com/TomyFernandez/JPAProyecto.git
2. **Compilar y ejecutar el Proyecto**:
  cd JPAProyecto
mvn clean install
mvn exec:java -Dexec.mainClass="org.example.Main"

3.**Verificar la Base de Datos**:

Abre la consola de H2 en tu navegador: http://localhost:8082
Conéctate a la base de datos utilizando las credenciales configuradas en persistence.xml.
Verifica que las tablas y los datos se han creado correctamente.

## Observaciones
1. **Creacion de h2**
 - Problema: La base de datos h2 no se conectaba al inicio por el siguiente error: Database: "C:/uUsers/nombreusuario/test" not found, either pre-create it or allow remote database creation (not recomended in secure environments)
  -Solucion: Crear un archivo en la ruta indicada de nombre test.mv y cambiarle el tipo de archivo a .db
2. **Incorporar el uso de Lombok al proyecto**
  -Problema: Debido a que en la lista de tutoriales de Youtube brindados por la catedra no utilizaba Lombok, el problema principal que se presento fue a la hora de utilizar Collecciones, ya que usando Lombok con la etiqueta @Builder no se inicializan las colleciones y esto presentaba el problema de que al usar los arraylist estos no estaban creados con anterioridad
  -Solucion: Utilizar la etiqueta @Builder.Default esto se soluciona pues ahora si se inicializan las colecciones y no marca error de punteros nulos

 

