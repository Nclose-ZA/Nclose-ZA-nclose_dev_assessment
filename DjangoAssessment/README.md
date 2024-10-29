# Django Backend Assessment

## Table of Content
- [Description](#description)
- [Preface](#preface)
- [Assignment](#assignment)

### Description
This is a basic Django assessment to gauge your personality is your code.
Complete the below [assignment](#assignment) while implementing good code practices as the entire approach, code and project will contribute to the outcome.
There is no time limit, but we believe this assignment should not take you longer than an hour or two.
Marks will be deducted for copy/paste code, including chatGPT. We will know ....
The goal is not to trip you up but rather to see how you approach an assignment and the end product you deliver.
Your repo must include a readme and changelog, with extra points for documentation.

### Preface
- On your personal Github account, create a public repo with the name of `django_assessment`.
- You can use as many or as few Python modules as you like.
- You can create as many branches and commits as you need, but we will only be reviewing your `production` branch.
- Once complete, you can send the link for us to clone and review.

### Assignment
- Create a new Django project with a mysql database that incorporates class based viewsets and utilizes Django Rest Framework for serialization.
- A docker-compose file has been provided for mysql.
- All views must be authenticated using session cookies.
- No templates are required.
- Extra points for group permission but not required.
- Core project
    + You have vendors, and each vendor has multiple products.
    + You have users and clients, each user can have multiple clients assigned to them.
    + Different users have different vendors assigned to them.
    + Add CRUD views for vendors, products, users and clients.
        - Products can be filtered by vendor
        - Clients can be filtered by user
        - Allow all products to be listed for a client.
    + Add any validation you believe is needed.
- External API
    + Create an endpoint for a user to retrieve formatted data from an external website.
    + This website collects phishing url's which can be used as part of threat intelligence for Cyber Security.
    + Download the latest file from the following [link](http://data.phishtank.com/data/online-valid.csv)
    + Convert the data to a serialized json object and return the response ready for the ui to display.
    + The data will be displayed in a table.
- A `mysqldump` with test data should be provided in a directory in or your repo.