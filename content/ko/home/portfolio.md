---
# A section created with the Portfolio widget.
# This section displays content from `content/project/`.
# See https://docs.hugoblox.com/widget/portfolio/
widget: portfolio

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 20

title: ''
subtitle: ''

content:
  # Page type to display. E.g. project.
  page_type: project

  # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
  filter_default: 0

  # Filter toolbar (optional).
  # Add or remove as many filters (`filter_button` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove the toolbar, delete the entire `filter_button` block.
  filter_button:
    - name: All
      tag: '*'
    - name: 프로젝트
      tag: PJ
    - name: 연구 
      tag: RE
    - name: 체크리스트
      tag: CL
    - dummy : 더미들
      tag: DM

design:
  columns: '1'
  view: grid    
  flip_alt_rows: false
  background: {}
  spacing: {padding: [5, 0, 5, 0]}
  border: {color: 'black', width: 3px, style: 'solid'}
  image_size: 'cover'
  image_style: 'border' 
---
