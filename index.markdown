---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Home
description: Kestrel is a open source project for web applications based on angular and nodejs / express. Join the project now !
last_modified_date: 2022-08-29 11:47
nav_order: 1
---

# Skulljs: A remastered version of Kestrel is available on [https://skulljs.github.io/](https://skulljs.github.io/)

---

# Focus on the code not the structure

Kestrel aims to give a solid structure to create a project based on Angular for the Frontend and ESM / Express / Sequelize for the backend.
{: .fs-6 .fw-300 }

[Get started now](/docs/getting_started){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [View it on GitHub](https://github.com/kestrel-org){: .btn .fs-5 .mb-4 .mb-md-0 }

---

Here is some features built in Kestrel:

## Utilities and cli

- The [kestrel-cli](https://www.npmjs.com/package/@kestrels/cli), several commands and utilities
- A customizable class named PDFGenerator for PDF generation
- Encryption functions to encrypt and decrypt strings with a AES - 256 protocol
- Optional use of Faker to populate the database with fake data
- A built-in support for sending mail
- An Angular directive to handle pre-loaders

## Authentication and security

- A built-in middleware for check if a user is logged
- A built-in middleware for verify a token through an authorization server
- Cors support
- A built-in security middleware using Helmet
- Session support using express-session

## Logs

- A built-in logger using Morgan

## Documentation

- Integration of Swagger for the backend
- Integration of Compodoc for the frontend

---

## About the project

Kestrel is &copy; 2021-{{ "now" | date: "%Y" }}

### License

Kestrel is distributed by an [MIT license](https://choosealicense.com/licenses/mit/).
