---
title: "Udev Rules"
date: 2022-05-18T18:15:53-04:00
draft: false
---

-   [Udev Rules](#udev-rules)
    -   [Requerimientos](#requerimientos)
    -   [Introducción](#introducción)
    -   [Cómo son organizadas las
        reglas](#cómo-son-organizadas-las-reglas)
    -   [Sintaxis de las reglas](#sintaxis-de-las-reglas)
    -   [Pandoc](#pandoc)

# Udev Rules

El objetivo de este tutorial es entender las reglas Udev en linux y
crear una regla práctica.

### Requerimientos

Tener permisos root de tu distro linux

### Introducción

En sistemas gnu/linux, mientras los dispositivos de bajo nivel son
manejados a nivel kernel. La administración de los eventos que guarda
relación con el espacio de usuario y es administrado por **udev**, para
ser más preciso con **udevd** daemon.

### Cómo son organizadas las reglas

Las reglas para **udev** son definidas dentro de archivos con la
extensión **.rules**, existen dos maneras de ubicar dichas reglas, dos
rutas que pueden ser las siguientes:

-   `/usr/lib/udev/rules.d`, siendo este primero el directorio principal
    para reglas del sistema.

-   Y `/etc/udev/rules.d` está reservado para las reglas creadas y
    customizada por el usuario.

Existe una convención para crear una regla, la cual es ser nombrado con
un número como prefijo y estas serán procesadas teniendo en cuenta un
órden léxico independientemente del directorio en el que se encuentre,
sin embargo las reglas custom pueden ser anuladas o sobreescritas con el
nombre instalada en el directorio por defecto.

### Sintaxis de las reglas

No es muy complicada una vez entendida la lógica que hay por detrás,
esta compuesta de dos secciones principales. La parte del *match*

### Pandoc

En el primer instante que conocí pandoc, dije que algún dia me serviría,
o probablemente es una autosugestión de que funcionó algo, tal como
esperabas y si existió algo de planeación debería ser **tal como lo
planeaba. Pero la alegria no durará mucho por la simple razón de que
habia hecho algo con tikz-pgf**
