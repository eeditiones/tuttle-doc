---
title: "how to use Tuttle?"
menuTitle: "how to use"
date: 2021-11-05T12:58:11+01:00
tags: []
---

{{% notice note %}}
in the pictures below the Github Logo is used but Gitlab can be used the same way
{{% /notice %}}


![Git 2 DB](/images/git2db.png)

### Git as the 'source of truth'

With 'Git to DB' editors will work with their own tools and push changes to Git. 
The data are kept in Git and are deployed to TEI-Publisher
on demand or automatically by an Git action. Data can be updated completely or incrementally just applying
the changes since last update.

There is a simple dashboard to trigger the updating of data and checking the status of connected repositories.

![DB 2 Git](/images/dashboard.png)

When opening the dashboard the status of the configured repositories is requested. The colors of
of the rows signal the status of the respective repository.

| color | Status |
| ----- | ------ |
| orange | new - the repository is configured but has not yet been deployed into TEI-Publisher. The 'incremental' button is disabled as the data need to be checked out before. |
| green | up-to-date - the are no differences between data in the database and the repository. 'Incremental' can be used to trigger update of differences. |
| blue | behind - the data in the database are behind the status in the repository. An update is needed |
| red | error - a configuration or connection problem occured |


