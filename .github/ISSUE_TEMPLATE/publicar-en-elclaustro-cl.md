---
name: Publicar en ElClaustro.cl
about: Describe brevemente de qué trata tu contenido (Opcional)
title: "[Título del contenido] "
labels: contenido
assignees: ngeorger

---

- type: markdown
    attributes:
      value: |
        Gracias por publicar en ElClaustro.cl!
  - type: input
    id: contact
    attributes:
      label: Datos de contacto
      description: Cómo podemos contactarnos contigo?
      placeholder: ejemplo: mail@correo.com (puede ser tu IG, etc)
    validations:
      required: true
  - type: textarea
    id: resumen
    attributes:
      label: Resumen del contenido
      description: Describe brevemente de qué trata tu contenido (Opcional)
      placeholder: Cuéntanos sobre tu post
      value: "Quiero publicar esta noticia!"
    validations:
      required: false
  - type: dropdown
    id: categoria
    attributes:
      label: Categoría
      description: En qué categoría va tu contenido?
      options:
        - Noticias
        - Discos Y Multimedia
        - Entrevistas
        - Columnas
    validations:
      required: true
  - type: textarea
    id: contenido
    attributes:
      label: post
      description: El contenido de tu mensaje
      render: markdown
