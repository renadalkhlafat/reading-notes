# Django form 
Django provides a Form class which is used to create HTML forms. It describes a form and how it works and appears 

Forms are basically used for taking input from the user in some manner and using that information for logical operations on databases

A process flowchart of how Django handles form requests is shown below, starting with a request for a page containing a form 
![form](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms/form_handling_-_standard.png)

## Declaring a Form
Form data is stored in an application's forms.py file, inside the application directory.

**Example:**
```python
from django import forms

class YourclassForm(forms.Form):
    renewal_date = forms.DateField(help_text="your message here.....(default 3).")
```