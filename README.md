# Aprendiendo lo Básico de Git

## Tabla de Contenidos
- [¿Qué es Git y para qué sirve?](#qué-es-git-y-para-qué-sirve)
  - [Características Principales](#características-principales)
- [Comandos Esenciales en Git](#comandos-esenciales-en-git)
  - [Inicializar Git en Nuestro Proyecto](#inicializar-git-en-nuestro-proyecto)
  - [Zona de Trabajo](#zona-de-trabajo)
  - [Verificar Estado de los Ficheros](#verificar-estado-de-los-ficheros)
- [Otros Comandos Útiles](#otros-comandos-útiles)
- [Recursos Adicionales](#recursos-adicionales)

# ¿Qué es Git y para qué sirve?
Git es un **sistema de control de versiones distribuido** que permite a los desarrolladores rastrear y gestionar cambios en el código fuente a lo largo del tiempo. Creado por **Linus Torvalds** en 2005 para el desarrollo del kernel de Linux, Git se ha convertido en una herramienta esencial en el desarrollo de software moderno.

### Características Principales:
- **Control de versiones:** Guarda distintas versiones del código, facilitando la comparación y restauración de versiones anteriores.
- **Colaboración:** Permite que múltiples desarrolladores trabajen simultáneamente en el mismo proyecto sin conflictos, gracias al uso de ramas.
- **Sistema distribuido:** Cada copia del repositorio contiene todo el historial del proyecto, permitiendo trabajar sin conexión y mejorando la redundancia.
- **Eficiencia:** Diseñado para ser rápido y manejar proyectos de cualquier tamaño con alta eficiencia.
<p>En resumen, Git es una herramienta esencial para el desarrollo moderno de software, proporcionando un entorno robusto para la gestión de cambios y la colaboración en proyectos de código fuente.</p>

> [!NOTE]
> Si aún no tienes Git instalado, puedes descargarlo desde la [página oficial de Git](https://git-scm.com/).

## Comandos Esenciales en Git

### Inicializar Git en Nuestro Proyecto:
Para comenzar a utilizar Git en un proyecto existente, abre tu terminal en la carpeta del proyecto y ejecuta:
```bash
git init
```

## Zona de trabajo:
Añadir archivos al área de preparación (staging area):
Agrega un archivo específico:
```bash
git add nombre_del_archivo
```
O agrega todos los cambios realizados:
```bash
git add . 
```

Realizar un commit con un mensaje descriptivo:
Guarda los cambios en el historial con un mensaje que describa lo que hiciste:
```bash
git commit -m "Mensaje descriptivo de los cambios" 
```

## Verificar Estado de los Ficheros:
Mostrar el estado de los archivos:
Te indica qué archivos han sido modificados, añadidos o eliminados:
```bash
git status
```

Ver el historial de commits:
Lista los commits realizados en el repositorio:
```bash
git log
```

Cambiar entre commits (checkout):
Puedes navegar a un commit específico usando su ID:
```bash
git checkout id_del_commit
```


## Otros comandos Útiles:
Cambiar de rama:
Para cambiar a la rama principal (por defecto "main"):
```bash
git switch main
```

Subir cambios al repositorio remoto:
Envía tus commits locales al repositorio remoto (asegúrate de tenerlo configurado):
```bash
git push
```

Actualizar tu repositorio local con cambios remotos:
Descarga y fusiona cambios del repositorio remoto:
```bash
git pull
```

Añadir etiqueta a un commit:
Asigna una etiqueta a un commit específico para marcar versiones:
```bash
git tag -a "v1.0" id_del_commit -m "Versión 1.0"
```

Restaurar cambios en archivos antes del commit:
Para descartar cambios en archivos específicos:
```bash
git restore nombre_del_archivo
```

Sacar archivos del área de preparación:
Si agregaste un archivo por error al staging area:
```bash
git restore --staged nombre_del_archivo
```

Comparar diferencias entre commits:
Muestra los cambios entre dos commits:
```bash
git diff id_commit1 id_commit2
```

Configurar VSCode como herramienta de diff:
Establece Visual Studio Code como tu herramienta de comparación por defecto:
```bash
git config --global diff.tool vscode
```

Usar la herramienta de diff para comparar cambios:
Abre VSCode para visualizar las diferencias:
```bash
git difftool id_commit1 id_commit2
```


## Recursos Adicionales
- [Documentación Oficial de Git](https://git-scm.com/doc?form=MG0AV3)
- [Pro Git Book (Español)](https://git-scm.com/book/es/v2?form=MG0AV3)


## Créditos

Este proyecto fue desarrollado por [s1lv3Dev](https://github.com/s1lv3Dev) con la ayuda de Microsoft Copilot.

---

> [!NOTE] 
> ¡Gracias por usar esta guía para aprender Git!
