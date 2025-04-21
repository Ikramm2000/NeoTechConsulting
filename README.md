# Task Assignment : Internship Roles in Low-Code, Automation & AI

## Part 1: Automate Contact Collection

**Workflow File:** [`auto_contact_collection_zap.json`](./Contatct_collection_zap.json)

**Tool Chosen**: Zapier  
I chose **Zapier** for its user friendly, no‑code interface and its drag-and-drop actions for Google Forms, Sheets, and Gmail.

**Duplicate Entries Handling**:  
To prevent duplicate entries:  
1. **Lookup Spreadsheet Row**: Search the Google Sheet for the submitted email.  
2. **Filter**: Proceed only if the email isn’t found.  
3. **Add Row**: Write data to the Sheet only after passing the filter.

**Resources**
- Google Form: [Contact Submission Form](https://docs.google.com/forms/d/e/1FAIpQLSfRP0vGM0AptfBE5TVtM3aAJHdJ9tB7CVnEjVCOi3Du6xeFXA/viewform?usp=header)
- Google Sheet: [Form Responses Sheet](https://docs.google.com/spreadsheets/d/1b2oaXDHNjEb8Sz950NKWIWWvY8DyxQS6bj4WJzmfQ1g/edit?usp=sharing)
