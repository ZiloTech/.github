# Welcome to Zilo GitHub


|Component|Status|
|--|--|
|Digital One Web App (Dev)|[![Deploy to Amazon ECS](https://github.com/ZiloTech/digital-one-web-app/actions/workflows/ecs-deploy.yml/badge.svg)](https://github.com/ZiloTech/digital-one-web-app/actions/workflows/ecs-deploy.yml)  |
|Digital Playground (Dev)|[![Digital Playground (dev)](https://github.com/ZiloTech/playground-telerik/actions/workflows/ecs-deploy.yml/badge.svg?branch=develop)](https://github.com/ZiloTech/playground-telerik/actions/workflows/ecs-deploy.yml)|







Below is some useful info you should read before either creating a new repo or looking to setup pipelines.

## Creating github pipelines (actions)

Re-Usable workflows should be considered where possible, if you need to do something unique and new in your pipeline consider creating a re-usable workflow so that others wishing to do the same thing can benefit - when creating please consider the guidance in the workflow repo : https://github.com/ZiloTech/infra-app-workflows



## Naming Repos

Naming a GitHub repo seems so simple - you'd just want something that is:

- Descriptive
- Readable
- Consistent
- Contextual
- Brief (short / succinct)




### Follow Conventions
Following the naming conventions that are established keeps every repo easily discoverable, sortable and helps fellow developers find things faster.
Github does not support the concept of groups or folders, with this in mind the following naming standard applies :

{product/area/concept}-{descriptive-repo-name}

The following standard prefix apply

- playground-{repo} : This is a prefix used to indicate this project is for POC, testing, messing about
- infra-{repo} : For lee to decide
- testing-{repo} : For Any test runners


### What about CamelCase?
The problem with camel case is that there are often different interpretations of words - for example, checkinService vs checkInService. Also, it is difficult with auto-completion if you have many similarly named repos to have to constantly check if the person who created the repo you care about used a certain breakdown of the upper and lower cases. It's also best to avoid upper case, no one likes yelling.

### Be specific
You may find you have to differentiate between similar ideas later.

- Use wildlife-locator-rest-service instead of locator-service or wildlife-rest-service.
- Be consistent. 
- How do you want your repositories to be sorted/grouped?

Without favouring any particular naming choice, remember that a git repo can be cloned into any root directory of your choice:

    git clone https://github.com/user/repo.git myDir

Here repo.git would be cloned into the myDir directory.

So even if your naming convention for a public repo ended up to be slightly incorrect, it would still be possible to fix it on the client side.

That is why, in a distributed environment where any client can do whatever he/she wants, there isn't really a naming convention for Git repo.
(except to reserve "xxx.git" for bare form of the repo 'xxx')

### Avoid Organization Monikers
Once established, it's a simple task to change repo names, BUT it can have unintended consequences like breaking downstream links - so think about a name that can be stable over a long period of time.  Ministry, Department, Agency, Division, Branch and team names are subject to change so it’s best to avoid including them as part of repo names.  Putting “BC” in the name is fine to provide the context of the “Province of British Columbia” but let’s not start every repo that way, it makes sorting and searching a pain.
