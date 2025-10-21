---
# Leave the homepage title empty to use the site title
title: 'Kevin Darío' # Nota: Si usas el archivo de autor 'admin' para tu nombre, puedes dejar esto vacío.
date: 2025-10-21 # Actualiza la fecha de creación/última revisión
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  # 1. BIOGRAFÍA Y RESUMEN
  - block: resume-biography-3
    content:
      # Asegúrate de que el nombre de usuario ('admin') apunte a tu perfil (Kevin Darío)
      username: admin
      text: ''
      # Botón para descargar CV
      button:
        text: Descargar CV
        url: uploads/resume.pdf
      # Dejamos estos títulos vacíos para no duplicar secciones de abajo
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Aplica un fondo de gradiente
      css_class: hbx-bg-gradient
      # Avatar customization
      avatar:
        size: medium 
        shape: circle 

  # 2. EXPERIENCIA (Toma el contenido de la carpeta 'experience')
  - block: collection
    id: work
    content:
      title: Experiencia Profesional
      filters:
        folders:
          - experience # Asume que tu experiencia está en esta carpeta
    design:
      view: list # Vista de lista
      columns: 1

  # 3. EDUCACIÓN (Toma el contenido de la carpeta 'courses' o 'education')
  - block: collection
    id: education
    content:
      title: Educación
      filters:
        folders:
          - education # Asume que tu educación está en esta carpeta
    design:
      view: list
      columns: 1

  # 4. HABILIDADES (Toma el contenido de la carpeta 'skills')
  - block: features
    content:
      title: Habilidades Técnicas
      # Si 'skills' está configurado en tu archivo de autor, se mostrará aquí
      # Si tienes la carpeta 'skills', usa 'block: collection' con 'folders: ['skills']'
    design:
      columns: '1'

  # 5. PREMIOS Y RECONOCIMIENTOS (Toma el contenido de la carpeta 'awards')
  - block: collection
    id: awards
    content:
      title: Premios y Reconocimientos
      filters:
        folders:
          - awards # Asume que tus premios están en esta carpeta
    design:
      view: list
      columns: 1

  # --- SECCIONES ELIMINADAS/REEMPLAZADAS ---
  # El bloque 'markdown' de "My Research" fue ELIMINADO ya que tu perfil de Kevin Darío lo reemplazó por la presentación profesional.
  # Los bloques de 'Publications', 'Talks', y 'News' fueron ELIMINADOS por ser académicos.

  # 6. CTA (Opcional - Recomiendo ELIMINAR EST
