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

**Improvement for Production**: 
Send confirmation email to user, Thank them and let them know their message was received.

**Resources**
- Google Form: [Contact Submission Form](https://docs.google.com/forms/d/e/1FAIpQLSfRP0vGM0AptfBE5TVtM3aAJHdJ9tB7CVnEjVCOi3Du6xeFXA/viewform?usp=header)
- Google Sheet: [Form Responses Sheet](https://docs.google.com/spreadsheets/d/1b2oaXDHNjEb8Sz950NKWIWWvY8DyxQS6bj4WJzmfQ1g/edit?usp=sharing)

## Part 2: ChatGPT Prompt
1. **Classification Prompt:**
```
Classify this response to "What interests you about our product?" into exactly one category:  
Price, Features, Support, or Other. Respond ONLY with the single category name.
```

2. **Examples**
   
  | Response                                  | Expected ChatGPT Reply |  
|----------------------------------------------------|------------------------|  
| "I wish the subscription were cheaper."            | Price                  |  
| "I really like the calendar integration."          | Features               |  
| "I need a 24/7 available support when something breaks." | Support            |  

3. **Workflow Integration** 

To integrate this step into the Part 1 workflow, I will insert it right after the “New or Updated Row in Google Sheets” trigger. Use the OpenAI (ChatGPT) app to classify the “response” using the prompt above. The model will return a category — one of: Price, Features, Support, or Other. Then, use a “Update Row” step to write that result into the "category" column in the same row, using the Row ID.  

## Part 3: Simple AI/ML & Data Science Task 
### The Notebook:
 [`iris_ml.ipynb`](./iris_ml.ipynb)
### Classification Report:
1. **Model Selection:**

We implemented a logistic regression model to classify iris species, chosen for its simplicity and effectiveness in handling multi-class classification.

2. **Test Accuracy:**

The model achieved 97% accuracy on the test set, demonstrating strong predictive capability with minimal complexity. 

3. **Improvement Idea:**

To further improve the model accuracy and  boost performance, I’d perform hyperparameter tuning via grid search with cross‑validation.
