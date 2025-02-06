# ¿Qué es Git y para qué sirve?
<p>Git es un sistema de control de versiones distribuido que permite a los desarrolladores rastrear y gestionar cambios en el código fuente a lo largo del tiempo. Fue creado por Linus Torvalds en 2005 para el desarrollo del kernel de Linux.</p>

## Principales características de Git:
<ul>
  <li>Control de versiones: Permite a los desarrolladores guardar distintas versiones de su código, facilitando la comparación y restauración de versiones anteriores.</li>
  <li>Colaboración: Facilita el trabajo en equipo, permitiendo que múltiples desarrolladores trabajen en el mismo proyecto sin conflictos, mediante el uso de ramas.</li>
  <li>Distribuido: Cada copia del repositorio contiene toda la historia del proyecto, permitiendo trabajar sin conexión y mejorar la redundancia.</li>
  <li>Eficiencia: Git está diseñado para ser rápido y manejar proyectos de cualquier tamaño con eficiencia.</li>
</ul>

<p>En resumen, Git es una herramienta esencial para el desarrollo moderno de software, proporcionando un entorno robusto para la gestión de cambios y la colaboración en proyectos de código fuente.</p>


> [!NOTE]
Si no tienes Git instalado, por favor descárgalo e instálalo desde [Git](https://git-scm.com/) antes de seguir los pasos a continuación.


## Comandos esenciales en Git

### Inicializar Git en nuestro Proyecto:

##### Inicializamos git en la ruta donde queremos el gestor de versiones:
```bash
git init
```

## Zona de trabajo:
##### Añadimos los archivo/s que queremos sincronizar con git:
```bash
git add
git add . 
```

##### Escribimos un mensaje cuando dentro del commit:
```bash
git commit -m "Escribir mensaje" 
```

## Verificar Estado de los Ficheros:

##### Información de estado de los archivos
```bash
git status
```

##### Muestra el historial de commits en un repositorio
```bash
git log
```

##### Elige una foto de los commit realizados
```bash
git checkout id_commit
```


## Otros comandos:

##### Elige una rama, la predeterminada “main”
```bash
git switch main
```

##### Desde el local sube al remoto
```bash
git push
```

##### Desde el remoto baja al local, para actualizar ficheros
```bash
git pull
```

##### Para añadir etiqueta a un commit
```bash
git tag "text" “id_commit”
```

##### Restaura fichero antes del staged
```bash
git restore . | nombre_fichero
```

##### Saca del staged el fichero
```bash
git restore --staged .\readme.md
```

##### Para poder comparar commits con Git
```bash
git diff id_commit id_commit
```

##### Configura VSCode para poder comparar commits dentro del editor
```bash
git config --global diff.tool vscode 
```

##### Para comprar los cambios de un commit u otro, y ver los cambios
```bash
git difftool id_commit id_commit
```
