# Questions and Answers

## Q1: What is the keyboard interaction missing?
- **Focus Navigation**: Due to the lack of appropriate focus styles and keyboard compatibility, users were unable to use the `Tab` key to browse through the accordion buttons.  
- **Collapse/Expand Using Enter and Space Keys**: One typical accessibility need for interactive components like buttons is the ability to switch between parts using the `Enter` and `Space` keys, which the accordion could not provide.

## Q2: What is the ARIA missing?
- **`aria-expanded`**: The buttons that indicated whether a section was expanded (`true`) or collapsed (`false`) lacked this feature.  
- **`aria-controls`**: Because each button was not linked to its associated content part using this attribute, screen readers were unable to connect the button to the collapsible area.  
- **`role="region"`**: The `region` role, which would have designated the content parts as landmark regions for screen readers, was absent.  
- **`aria-labelledby`**: The content sections lacked this feature, which would have connected them to the appropriate buttons for screen reader users.
