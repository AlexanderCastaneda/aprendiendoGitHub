name: 💡 Mejora de código
description: Sugerencia para mejorar partes del código existente.
title: "[SUGERENCIA]: "
labels: ["mejora", "refactor", "optimización"]
assignees:
  - tu_usuario_github

body:
  - type: markdown
    attributes:
      value: |
        ¡Gracias por contribuir con una sugerencia para mejorar el código! Por favor llena los siguientes campos:

  - type: input
    id: archivo
    attributes:
      label: 📁 Archivo o módulo afectado
      description: Especifica en qué archivo o módulo se encuentra la parte del código a mejorar.
      placeholder: src/componentes/UsuarioController.java
    validations:
      required: true

  - type: textarea
    id: descripcion
    attributes:
      label: 📝 Descripción de la mejora propuesta
      description: Explica claramente cuál es la mejora y por qué sería útil implementarla.
      placeholder: Mejorar el uso de bucles en la función renderUsuarios para aumentar la eficiencia...
    validations:
      required: true

  - type: textarea
    id: justificacion
    attributes:
      label: 🔍 Justificación técnica
      description: ¿Cuál es el motivo técnico para esta mejora? ¿Se alinea con buenas prácticas, patrones de diseño, rendimiento?
      placeholder: El método actual tiene una complejidad O(n²), lo cual podría afectar el rendimiento con grandes volúmenes de datos...
    validations:
      required: true

  - type: textarea
    id: solucion
    attributes:
      label: 💡 Posible solución o referencia
      description: (Opcional) Si tienes una idea de cómo resolverlo o conoces documentación que lo respalde, compártela aquí.
      placeholder: Podríamos implementar un diccionario en lugar de recorrer la lista dos veces...
    validations:
      required: false

  - type: dropdown
    id: prioridad
    attributes:
      label: 🚦 Prioridad sugerida
      description: ¿Qué tan urgente o beneficiosa consideras que es esta mejora?
      options:
        - Alta
        - Media
        - Baja
      default: 1