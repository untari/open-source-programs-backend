---
id: Code-Organization
title: Code Organization
---

This page will give you a general overview of OSP architecture. As any other Django project Portal organizes its functionality in several apps:

- docs - contains the Postman collection `.json` file, which includes API docs and tests
- main - includes settings and URLs for the whole application, list of all apps, default requirements and so on
- token_auth - showing and editing user personal profile.
- osp - contains the working of the forms and questions; and related models, serializers & views.

Each app along with models, views, URLs, and other app-related code (admin, utils) contains a folder with migrations and tests. The migrations are generated by Django and shouldn't be edited manually.

The frontend code for this application can be found [here](https://github.com/anitab-org/anitab-forms-web).
