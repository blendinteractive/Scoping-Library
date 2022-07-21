# Accordion

A series of collapsible areas connected in a way that keeps only one open at a time.

For accordion expanding, an accordion "wrapper" or "container" needs to be included.

### Functional Specifications

Individual collapsible areas are activated open or closed by clicking/touching the interaction area - the entire title and expand/collapse icon. When open, the main content area is _not clickable/tappable_ for the interaction.

An individual collapsible area is a unique component that includes a title (heading, which acts as the interaction) and both a rich-text editor and component area. Heading titles can be adjusted based on editorial needs.

Accordions are grouped using an accordion group component, which groups collapsible areas so that the accordion (one open, the rest closed) works as expected.

### Additional Functionality



### Content Model

* Title
* Rich-Text
* Component Area

### Estimate Hours

TK

### Build Plan

TK

### Example

### Testing Scenario

1. Accordion group can only be placed on required pages
2. Only Accordion child items are placable within the Accordion group
3. Accordion child item Title is editable and title appears on the front-end
4. When active (clicked/focus with enter) the Accordion item opens while the other items close
5. A focus state is visible when tabbing through the Accordion item titles
6. Only the scoped content is available to be placed within an Accordion item. Typically this is a WYSIWYG field or media

### Ongoing Notes
