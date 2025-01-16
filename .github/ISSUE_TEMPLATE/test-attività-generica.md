name: Attività Generica
description: Traccia un'attività generale da svolgere nel competence center
title: "[Task] Titolo attività"
labels: ["task", "priority"]
assignees: []

body:
  - type: markdown
    attributes:
      value: |
        **Descrizione dell'attività**
        Fornisci un contesto chiaro e dettagliato per questa attività.
  
  - type: textarea
    id: descrizione
    attributes:
      label: Descrizione
      description: Specifica i dettagli dell'attività, i suoi obiettivi e i risultati attesi.
      placeholder: Descrizione dell'attività...
    validations:
      required: true
  
  - type: select
    id: priorità
    attributes:
      label: Priorità
      description: Assegna una priorità a questa attività.
      options:
        - Alta
        - Media
        - Bassa
    validations:
      required: true
  
  - type: input
    id: scadenza
    attributes:
      label: Scadenza
      description: Inserisci una data di scadenza (se applicabile).
      placeholder: YYYY-MM-DD
  
  - type: checkboxes
    id: checklist
    attributes:
      label: Sottocompiti
      description: Aggiungi eventuali sottocompiti per questa attività.
      options:
        - label: Compito 1
        - label: Compito 2
        - label: Compito 3
