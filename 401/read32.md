# Serverless and Amplify

* Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers.
* A serverless application runs in stateless compute containers that are event-triggered, ephemeral (may last for one invocation), and fully managed by the cloud provider.
* Pricing is based on the number of executions rather than pre-purchased compute capacity.
* Serverless applications are event-driven cloud-based systems where application development rely solely on a combination of third-party services, client-side logic and cloud-hosted remote procedure calls (Functions as a Service).
* One of the major advantages of using Serverless is reduced cost
* The downside is that Serverless functions are accessed only as private APIs.
* To access these you must set up an API Gateway.
* This doesn’t have an impact on your pricing or process, but it means you cannot directly access them through the usual IP.
* Setting up different environments for Serverless is as easy as setting up a single environment.
* With Serverless computing, there’s a hard 300-second timeout limit.
* Scaling process for Serverless is automatic and seamless, but there is a lack of control or entire absence of control.
* FaaS is an implementation of Serverless architectures where engineers can deploy an individual function or a piece of business logic.
* With Serverless, everything is stateless, you can’t save a file to disk on one execution of your function and expect it to be there at the next.
* FaaS are designed to spin up quickly, do their work and then shut down again.
* With stateless functions multiple containers can be initialised, allowing as many functions to be run (in parallel, if necessary) as needed to continually service all incoming requests.
* A Serverless solution consists of :
  * a web server
  * Lambda functions (FaaS)
  * security token service (STS)
  * user authentication
  * database.

## AWS

* AWS Amplify is a set of tools and services that can be used together or on their own, to help front-end web and mobile developers build scalable full stack applications, powered by AWS. 
* With Amplify, you can configure app backends and connect your app in minutes, deploy static web apps in a few clicks, and easily manage app content outside the AWS console.
* Amplify supports popular web frameworks including JavaScript, React, Angular, Vue, Next.js, and mobile platforms including Android, iOS, React Native, Ionic, Flutter. 

## Benefits

* Configure backends fast
* Seamlessly connect frontends
* Deploy in a few clicks
* Easily manage content

# API (GRAPHQL)

* The GraphQL Transform provides a simple to use abstraction that helps you quickly create backends for your web and mobile applications on AWS.
* With the GraphQL Transform, you define your application's data model using the GraphQL Schema Definition Language (SDL) and the library handles converting your SDL definition into a set of fully descriptive AWS CloudFormation templates that implement your data model.
