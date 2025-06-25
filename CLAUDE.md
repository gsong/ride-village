## TaskMaster Workflow

- PRD: @docs/prd.md
- Estimate 5-20 tasks based on PRD complexity before parsing
- When editing the PRD (docs/prd.md), always follow the structure and sections from .taskmaster/templates/example_prd.txt as a formatting guide

## Project Management

- Project board: `gh project view 5 --owner gsong`

### Moving Issues to "Up Next" on Project Board

1. Get project items: `gh project item-list 5 --owner gsong --format json`
2. Find the item ID for the issue you want to move
3. Move to "Up Next": `gh project item-edit --id <ITEM_ID> --project-id PVT_kwHOAAlEvM4A8U2f --field-id PVTSSF_lAHOAAlEvM4A8U2fzgwW8Is --single-select-option-id 215cacf3`

**Project Constants:**
- Project ID: `PVT_kwHOAAlEvM4A8U2f`
- Status Field ID: `PVTSSF_lAHOAAlEvM4A8U2fzgwW8Is`
- "Up Next" Option ID: `215cacf3`
