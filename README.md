# 2.13-assignment
Make a comparison between Serverless Framework and Terraform as tools for IaC. answer the following:

1	What type of infrastructure and application deployments are each tool best suited for?

Serverless Framework is ideal for serverless applications, particularly those running on cloud platforms like AWS Lambda. It removes the need to manage servers, allowing developers to focus on writing functions instead of handling infrastructure.

Terraform is ideal for managing a wide variety of infrastructure, including virtual machines, databases, Kubernetes clusters, and cloud services like AWS. It isn't limited to serverless environments and can handle any type of infrastructure resource.

2	How do their primary objectives differ?

The Serverless Framework simplifies the deployment and management of serverless applications, focusing on code deployment with minimal infrastructure management.

Terraform is a broader tool for managing the entire lifecycle of infrastructure. It can provision and manage any resource, whether in the cloud or on-premises, and ensures the infrastructure remains in a desired state.

3	How do they differ in terms of learning curve and ease of use for developers or DevOps teams?

The Serverless Framework has a relatively easy learning curve for developers familiar with serverless technologies, especially AWS Lambda. It simplifies serverless configurations and allows developers to deploy code with minimal focus on infrastructure, using high-level YAML/JSON files.

Terraform has a steeper learning curve, particularly for those new to infrastructure concepts. It requires understanding HashiCorp Configuration Language (HCL) and managing resources across cloud providers. While powerful and flexible, it demands a deeper understanding of infrastructure, making it easier for DevOps teams but more challenging for developers focused on application code.

4	What are the differences in how each tool handles state tracking and deployment changes?

The Serverless Framework relies on the cloud platform's state management (e.g., AWS CloudFormation) to track state automatically, so developers don't need to manage it manually. It updates resources incrementally, typically updating functions and event triggers without affecting other resources unless needed.

Terraform tracks state using a state file, which helps determine what changes are required during deployment. When you run terraform apply, it compares the current infrastructure with the desired state and makes the necessary changes, such as creating, modifying, or destroying resources based on the difference.

5	In what scenarios would you recommend using Serverless Framework over Terraform, and vice versa?

Use the Serverless Framework when:
	Building serverless applications (e.g., Lambda, API Gateway, DynamoDB).
	Focusing on code and event-driven architectures without managing infrastructure.
	Deploying functions with a simplified serverless management experience.
	Targeting cloud-native platforms like AWS that support serverless services.

Use Terraform when:
	Managing a wide range of infrastructure resources (e.g., compute, storage, databases, Kubernetes).
	Deploying complex or hybrid cloud environments (including serverless with broader infrastructure needs).
	Managing resources across multiple cloud providers or on-premises.
	Needing state-driven, version-controlled, and customizable infrastructure management.

6	Are there scenarios using both together might be beneficial?

Combining Serverless Framework with Terraform is useful for hybrid architectures where part of your app is serverless (e.g., AWS Lambda) and part requires traditional infrastructure (e.g., VPCs, EC2, Kubernetes).

Use Terraform to manage the overall infrastructure (like networking and databases) and use the Serverless Framework for deploying serverless functions and services (e.g., API Gateway, DynamoDB, Lambda). This way, you can take advantage of Terraform’ s broader infrastructure management and Serverless Framework’s simplicity for serverless applications.

Create a public github repository that has a README.md file, containing the above answers.
Submission is the url to your public github repository.
https://github.com/tschui7745/2.13-assignment

