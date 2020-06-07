---
to: 2019-03-01
company: COST Association
icon: flask
sector: Nonprofit Organization
---

COST – European Cooperation in Science and Technology – is an EU-funded programme that enables researchers to set up their interdisciplinary research networks in Europe and beyond. We provide funds for organizing conferences, meetings, training schools, short scientific exchanges or other networking activities in a wide range of scientific topics. By creating open spaces where people and ideas can grow, we unlock the full potential of science.

The IS Team Unit is in charge of the accounting tool, named e-COST, that helps the organization achieving those goals.

The current challenge is mostly to refresh a years old application while continuing to deliver new functionalities.

In the past years, we achieved:
- to operate a smooth transition from SVN to git, for a better branching experience
- the switch from bugzilla to Jira Agile, to strengthen our Agile needs of working
- to introduce Symfony in the legacy and fully custom application
- to introduce Docker, in order to facilitate the possibilities to introduce breaking changes, even on the infrastructure level
- to fully review our continuous integration system, moving it from TeamCity to bamboo
- to introduce dependencies manager, for front and back end dependencies — composer, for Symfony, but also for legacy, and yarn, used along with WebPack Encore
- to introduce a front end framework (bootstrap) in order to have a smoother UX and UI for our end users, and possibly to go full responsive
- to fully replace our mail testing environment by switching from shared mailboxes and application level mail redirection to Mail Hog, a pretty easy to use and configure mail catcher
- to introduce industry level good practices such as pull request — thanks to Bitbucket, the usage of code style standards — thanks to PSR and Code Sniffer, and a general awareness upon code quality — with a recent addition of Mess Detector
- to have a full CI/CD based on Bitbucket Pipelines that pushes Docker images to AWS ECR and deploys to ECS all this automated with CloudFormation