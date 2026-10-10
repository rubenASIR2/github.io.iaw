# Ejercicio 5: Creación de un sitio con GitHubPages

## 1. Creación del repositorio

*En primer lugar, accedí a mi cuenta de GitHub y creé un nuevo repositorio  llamado iaw, donde voy a guardar los ejercicios realizados anteriormente en la asignatura de Implantación de Aplicaciones Web*

![Ejercicio5captura1](images1/Creacionrepositorioiaw1.png)
![Ejercicio5captura2](images1/Repositorioiawcreado.png)




## 2. Creación de la rama gh-pages

*Una vez creado el repositorio, creé una rama llamada gh-pages, que será la encargada de publicar el sitio web mediante GitHub Pages.*

*Esta rama se utilizará como fuente de publicación y tendrá como directorio de origen la raíz del repositorio*

*Lo realizaremos todo por terminal*

![Ejercicio5captura3](images1/Creacionramagh-pages.png)



## 3. Clonación de los repositorios 

*Para trabajar con los archivos desde mi equipo, cloné el repositorio original y el nuevo repositorio utilizando los siguientes comandos:*

```bash

$ git clone https://USERNAME:TOKEN@github.com/USERNAME/REPO.git
```
*El comando descarga el repositorio original lo clona*

## 4. Copia de los archivos 

*Después de clonar los repositorios, copié los archivos de los ejercicios que tenía realizados en el repositorio original al nuevo repositorio `iaw`.* 
*posdata: reordene todo un poco*

![Ejercicio5captura5](images1/Reorganizacion%20de%20directorio2.png)


*Organicé los documentos siguiendo la estructura solicitada en el enunciado:*


*iaw/
├── README.md
└── activididad1_1/
    ├── ejercicio1.md
    ├── ejercicio2.md
    ├── ejercicio3.md
    ├── ejercicio4.md
    └── img/*


*Los cuatro ejercicios se encuentran dentro de la carpeta actividad1*

## 5. Creación del indice de contenidos 

*En el directorio raíz de la rama gh-pages, creé el archivo README.md, que servirá como página de inicio del sitio web*


*Para crear los enlaces utilicé la sintaxis de Markdown rutas relativas:*

- [Ejercicio1](actividad1_1/ejercicio1.md)
- [Ejercicio2](actividad1_1/ejercicio2.md)
- [Ejercicio3](actividad1_1/ejercicio3.md)
- [Ejercicio4](actividad1_1/ejercicio4.md)

*De esta forma, al pulsar sobre cada enlace, se puede acceder al documento correspondiente.*

## 6. Subida de los archivos a GitHub

*Una vez organizados los archivos, abrí una terminal dentro de la carpeta del nuevo repositorio y ejecuté los siguientes comandos:*

```bash
git switch gh-pages
git add README.md actividad1_1
git commit -m "Añadir ejercicios de IAW"
git push origin gh-pages
```
![Ejercicio5Captura6](images1/Subida%20de%20archivos%20a%20GitHub.png)
![Ejercicio5Captura7](images1/gitcommitcasifinal.png)
![Ejercicio5Captura8](images1/Gitpushorigingh-pages.png)



*Con estos comandos añadi los archivos a Git, guardé los cambios mediante una confirmación y los subí a la rama gh-pages del repositorio remoto*

![Ejercicio5Captura9](images1/Comprobacion%20de%20los%20cambios%20hechos%20en%20github.png)

## 7. Configuración de GitHub Pages

*Para publicar el sitio web, accedí a la configuración del repositorio y seguí estos pasos:*

``` bash 
1. Entre en **Settings**.
2. Accedí al apartado **Pages**.
3. En la sección **Build and deployment**, seleccioné **Deploy from a branch**.
4. Elegí la rama gh-pages como fuente de publicación.
5. Seleccioné la carpeta /root.
6. Pulsé **Save** para guardar los cambios.
```

## 8. Comprobación del sitio web

*Por último, comprobé que GitHub Pages publicara correctamente el sitio web y que la página principal 
mostrara el índice de los ejercicios*

*La dirección del sitio web es:*

[https://rubenASIR2.github.io/iaw/](https://rubenASIR2.github.io/iaw/)

*También comprobé que los enlaces a los ejercicios dirigieran a los documentos correspondientes y que las imágenes,en caso de utilizarlas, se mostraran correctamente*.










