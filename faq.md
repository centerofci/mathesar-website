---
layout: faq
title: FAQ - Mathesar
---

{% capture faq_section1 %}

### Can I create and share forms using Mathesar?

Not yet, but they're [on our roadmap](roadmap.html).

### What kind of access control does Mathesar support?

Mathesar currently supports *Manager*, *Editor*, and *Viewer* roles on per-schema and per-database. *Managers* can edit the structure of the database, *Editors* can edit data (but not the database structure), and *Viewers* have read-only permissions.

More granular permissions - including row and column level permissions - are [on our roadmap](roadmap.html).

### Do you support using formulas to calculate data automatically?

Not yet, but we've done some early design work on this and it is [on our roadmap](roadmap.html).

{% endcapture %}

{% capture faq_section2 %}

### How is Mathesar different from a spreadsheet?

Spreadsheets are easy to use, but they’re also easy to mis-use because they're so unstructured.

This lack of structure can leave spreadsheet users without answers to these questions:

- How can I prevent entry of duplicate data into my spreadsheet?
- How do I quickly store and visualize the relationships between my data?
- How do I evolve the structure of my data as my needs change?

These problems can be solved by databases.

Mathesar is about halfway between a database and spreadsheet.
Like a database, Mathesar’s interface can provide structure – so your team can’t mistakenly enter inaccurate data. This helps ensure that your data is consistent and clean.

And like a spreadsheet, Mathesar has an accessible beginner-friendly interface.

### How is Mathesar different from Airtable?

Airtable is a mature solution and offers more features than Mathesar. That said, Mathesar offers you multiple advantages:

- Mathesar is open source and self-hosted – you can run it on your own servers.
- You can connect to your Mathesar database and run SQL queries.
- You can use Mathesar alongside the ecosystem of Postgres tools, i.e. you don’t have to depend on the integrations that Airtable allows for.
- You can keep your data even if you stop using Mathesar. Your data is separate from the interface and is therefore in your ownership.
- Mathesar allows you to ensure stronger data **validation** and data **integrity** (clean, consistent data).
- **Changing** your data models in Mathesar can take you just a few clicks. Whereas Airtable’s reconfiguration process is much more limited.
- Mathesar’s Data Explorer lets you create **views from multiple tables** easily. Airtable does not currently offer this feature.

These points also apply to similar cloud-based solutions – including SeaTable, Google Tables and Microsoft Lists.

### How is Mathesar different from NocoDB?

We firmly believe that the more open-source tools, the better! So we have lots of respect for the NocoDB team’s accomplishments.

Both Mathesar and NocoDB provide an interface to existing databases, but here’s how we take a different approach:

- Mathesar is a UI to PostgreSQL databases. Whereas NocoDB supports connecting to MySQL, MSSQL, and SQLite DBs. This means that Mathesar can support PostgreSQL features at a richer level.
- Mathesar’s UI is built directly around the features within Postgres. There are no abstractions that could prevent users from working with the same data in other tools outside Mathesar.
- Relationships set up in Mathesar’s UI will reflect at the database level Mathesar’s UX can help you understand underlying relationships in your data.
- Mathesar’s Data Explorer lets you build queries across multiple tables. NocoDB doesn’t currently offer this feature.
- Changing your data models in Mathesar can take you just a few clicks .Schema migrations in NocoDB involve a manual process.

Note: NocoDB is a more mature solution than Mathesar and supports features like webhooks, integrations, notifications, etc. that Mathesar does not currently support.

Please see our roadmap for more info on Mathesar’s upcoming features.

### How is Mathesar different from Baserow?

They’re both open source tools, but Mathesar’s approach is different from Baserow:

- You cannot connect an existing database to Baserow – whereas you can connect your Postgres database to Mathesar.
- Relationships in Baserow do not reflect at the database level. Baserow has its own abstractions so what shows up as a "linked field" is not actually a database relationship. Mathesar has no abstractions. What you see in the UI is what you get in the database.
- You cannot make views across different tables using Baserow. Whereas Mathesar’s Data Explorer allows you to see one view of different tables in your database.
- Baserow has some paid premium features, even for self-hosted installations. All of - Mathesar's features are available for free.

Note: Baserow is a more mature project than Mathesar and supports features like plugins, real-time collaboration, etc that Mathesar does not currently support.

Please see our roadmap for more info on Mathesar’s upcoming features.
{% endcapture %}


{% include faq_section.html content=faq_section1 section="Features" %}
{% include faq_section.html content=faq_section2 section="Product Comparisons" %}
