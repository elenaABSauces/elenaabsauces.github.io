---
layout: post
read_time: true
show_date: true
title: "Caso Práctico"
date: 2021-2-31
img: posts/20211105/practico.png
tags: [jekyll, web, aplicación]
author: Elena de Antón
description: "Caso practico"
---

## EXPLICACIÓN DEL TRABAJO REALIZADO
A lo largo de este proyecto, se ha investigado el funcionamiento de Jekyll como generador de webs estáticas, y como alojar una web en GitHub Pages.
Primero, he evaluado las diferentes herramientas que podía utilizar para la realización de este proyecto: entornos de desarrollo, gestores de contenidos, generadores de páginas webs estáticas y opciones de alojamiento web.
Tras decantarme por la herramienta de Jekyll como generador de webs estáticas, realicé un repaso por la documentación existente en internet y que facilita la propia página web de Jekyll. Una vez entendí el proceso y las ventajas que me ofrecía el uso de Jekyll con GitHub Pages, decidí crear mi propia web utilizando uno de los temas de Jekyll, y alojarla de forma gratuita en GitHub Pages.
En dicha web, se puede encontrar la documentación contenida en este proyecto para que cualquier persona pueda seguirlo como guía y publicar su propia página web utilizando Jekyll.
	REPOSITORIO DE SOFTWARE
He utilizado GitHub como repositorio de software y sistema de control de versiones. El repositorio es de código abierto y se puede encontrar en el siguiente enlace: 
https://github.com/elenaABSauces/elenaabsauces.github.io
Este mismo repositorio, se utiliza como base para el alojamiento en GitHub Pages.

## DOCUMENTACIÓN: MANUAL DE USUARIO, MANUAL DE DESPLIEGUE

Pre-requisitos:
Jekyll recomienda utilizar Linux o macOS. A pesar de eso, y aunque Windows no es una plataforma oficial, se puede utilizar Windows con Jekyll realizando los siguientes pasos:
1º Instalar RubyInstaller para instalar Ruby: https://rubyinstaller.org/downloads/
•	 Ruby+Devkit 3.0.2-1 (x64) 
Y seguir con los pasos del “installation wizard”:

<center><img src="./assets/img/posts/20211031/ruby1.png" width="480px"></center>

Después de la instalación, cierro y abro una nueva terminal de comandos para instalar las gemas de Jekyll y Bundler:
gem install jekyll bundler
Para comprobar que está instalado correctamente utilizamos el comando jekyll -v

<center><img src="./assets/img/posts/20211031/ruby2.png" width="480px"></center>


También se puede ejecutar el comando de instalación de Jekyll directamente sobre la carpeta que hemos clonado del repositorio con la plantilla que vamos a utilizar

<center><img src="./assets/img/posts/20211031/ruby3.png" width="480px"></center>

Dentro de la carpeta del proyecto, para generar la página web se pueden utilizar los co-mandos:
jekyll serve (para una carga inmediata
jekyll serve –watch para que la web se sincronice y vaya mostrando los cambios a me-dida que vas trabajando y guardando el proyecto.
El comando jekyll serve mostrara en la terminal el puerto local en el que puedes ver tu página web. Por defecto, Jekyll usa el puerto 4000, pero puedes modificarlo usando --port:
Jekyll serve - –port 4001

<center><img src="./assets/img/posts/20211031/ruby4.png" width="480px"></center>

Si se utiliza la versión de Ruby 3.0.0 o superior, requiere añadir manualmente la depen-dencia webrick en el gemfile:
gem "webrick", "~> 1.7"

<center><img src="./assets/img/posts/20211031/ruby5.png" width="480px"></center>

Para utilizar una plantilla de Jekyll, tan solo tenemos que hacer un fork de ella en nuestro repositorio de GitHub. Si la vamos a desplegar en GitHub Pages, cambiaremos el nombre de dicho repositorio a nuestro nombre de usuario.github.io
También se puede pulsar directamente a “use this template”, y os aparecerá directamente para añadir esta plantilla a vuestra GitHub Pages:

<center><img src="./assets/img/posts/20211031/github1.png" width="480px"></center>

Configuración de GitHub Pages:

<center><img src="./assets/img/posts/20211031/github2.png" width="480px"></center>

Fork en nuestro repositorio:

<center><img src="./assets/img/posts/20211031/github3.png" width="480px"></center>

A partir de este momento, podemos realizar cambios directamente en el repositorio y utili-zarlo como entorno de desarrollo.
En nuestro caso, hemos decidido realizar un desarrollo en local, por lo que clonaremos dicho repositorio y comenzaremos a trabajar en él desde nuestro IDE.
Lo más importante es cambiar y personalizar el fichero _config.yml.

<center><img src="./assets/img/posts/20211031/vs.png" width="480px"></center>


Segundo, recomiendo cambiar las imágenes de la carpeta de assets/img por las que queramos nosotros, el diseño y los colores en /assets/css/main.css o cualquier otro cambio que queramos realizar para personalizar la plantilla a nuestro gusto.
En este caso, se han modificado los ficheros alojados en la carpeta _posts para crear las diferentes entradas de la web.


Además de todos estos cambios en el código, también se pueden añadir diferentes wid-gets.
Nuestra plantilla, utiliza widgets tanto para la Newsletter como para los comentarios:

<center><img src="./assets/img/posts/20211031/comentarios.png" width="480px"></center>

Como ya estaban por defecto, lo único que hemos tenido que hacer es crear una cuenta en  https://mailchimp.com para tener activo el Newsletter

<a href="https://mailchimp.com"><img  src="./assets/img/posts/20211031/mailchimp.png" width="240px"></a>

y en https://disqus.com/ para activar los comentarios y poder moderarlos.

<a href="https://disqus.com"><img  src="./assets/img/posts/20211031/disqus.png" width="240px"></a>

