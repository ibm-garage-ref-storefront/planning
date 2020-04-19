# Planning

- Use Storefront (updated version of bluecompute) as Cloudnative reference architecture.
- Enable appsody stacks.
- Each repo will use icp4apps/kabanero pipelines.
- Use cloud native tool kit as part of the app.
- Deploy the app using MCM
- Refactoring the databases keeping the open shift operators in mind.
- Get the app done in Spring, MicroProfile, OpenLiberty, Quarkus.
- Update the architecture center with the new reference architecture.

# Repo structure

- Creating a new org under public GitHub.
- Create individual repos for each micro service version with two branches one covering the appsody enabled service and other one containing the existing plain structure.
- One micro service will in turn have their own individual repos for each version of it like Spring, MicroProfile, OpenLiberty, Quarkus etc
- One repo for GitOps for each microservice having all the kube yamls. These yamls will be modified by the CI based on the tasks.
- One repo for devops covering the pipelines for all the microservices.
- One repo for MCM covering rescources that are used to deploy the application on multiple clusters
