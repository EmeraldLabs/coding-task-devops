Ground Rules
=======
* We prefer well-thought-out solutions over the quick-and-dirty kind. So take your time, if you need it. A rushed job is usually matched by a swift rejection.

Context
=======
We have developed this web application, and it contains the following features:

 - Member sign up/sign in
 - Manage Todo / add / edit / list / delete

The application was developed using node.js, and it requires a database - mongodb - for storing data. 

Problem
=======
As an architect, you decide to deploy the application on AWS using Kubernetes and use Mongodb as the database and it should support HA (high availability).

Instructions
===========
 - Using Terraform, build the infra-structure resources such as vpc, subnets, instances, elb, security group and etc., in the most optimal way with Production Grade security measures.
 - Build a Kubernetes Cluster in this VPC in an internal subnet. Try avoiding cloud provided services such as EKS/AKS/GKE.
 - You may need to modify the application source code or configuration in order to make the application running on Kubernetes cluster, e.g. make use ENV variables in 12Factor style, create Dockerfile.
 - Build the Docker image using GitHub actions / Circle CI / Drone CI etc.
 - Maintain the Docker Image in private reposritory such as Docker Hub, ECR and etc.
 - Build the Helm charts with configmaps, deployments, services and etc. for the application.
 - Deploy the MongoDB on either Kubernetes/EC2 with High Availability mode (master/slave) and configure it with the Application.
 - Deploy any choice of CD tools such as Jenkins, Travis and etc using Ansible / Saltstack.
 - Build Groovy scripts to create Jenkins Jobs or similar.
 - Deploy the Ingress controller such as Traefik / Kong and configure the Ingress accordingly.
 - Make sure to not have any manual installations rather use configuration managers such as Ansible / Saltstack etc.
 - Review your solution and ensure it follows best practices of building and deploying microservices.
 - Prepare a detailed document and/or instructions about what you have done. This documents must detail steps for other DevOps Engineer to understand how to deploy this application and maintain it.

Suggested tools
=======
You can use - not limited to - this tools in your solution:
- Terraform
- Ansible / Saltstack
- Docker
- Kubernetes
- Kustomize / Helm v3
- Kong Ingress Controller / Traefik v2 IngressRoute
- Mongodb v4
- Jenkins / Travis
- Github Actions / Circle CI / Drone CI

Expected outcome
=====
We expect to you deliver a high quality solution that allow us to:
- Build and manager the infrastructure on AWS
- Bundle and Build the application automatically on successful code changes
- Bootstrap kubernetes cluster with all services needed to run the application
- Deploy and manage the database on Kubernetes / EC2 smoothly
- Deploy Kong Ingress Controller / Traefik IngressRoute and discover the service
- Deploy the application on Kubernetes so external customers start using it.

Implementation guideline
=========
Please follow this guidelines while implementing the solution.

- Solution and code should be descriptive and well documented.
- Methods, variable naming and casing should be clear and consistent.
- Integrate CI/CD Service such as “travis” or github actions and add status badge in README.
- Write clear README with installation and testing steps.

How to proceed
===========
1) Clone this repository on your local machine and start a new local repository.
2) Write the code.
3) Write the documentation.
4) The repository should contains the modified application and all other DevOps files and scripts in a separate folder
4) Create a Private Project on Github and push your code on it. And give the access to following users: [Meabed](https://github.com/meabed)

Time limit
===========
There is no time limit as long as the job position remains vacant.

Final step
===========
Successful candidates will be invited to an in-person interview.
We may ask you more details of your code choices.
