### Domain 1: SDLC Automation
#### Implement CI/CD pipelines.
**SDLC lifecycle**
1. Define requirement, goal, and timelines.
2. Create a design plan.
    - includes: entire architecture, features, infrastructure requirement, user interface, and security.
3. Create source code.
4. Add testing.
5. Deploy the tested version.
6. Setup automation, monitor, and add new features.

CI/CD is a set of practices and methods that speed up the software delivery by adding automation into SDLC.
![alt text](image.png)

![alt text](image-4.png)

![alt text](image-2.png)

![alt text](image-3.png)


#### 1.2 Integrate automated testing into CI/CD pipelines.
- Review automated testing in the exam prep for Developer Associate

![alt text](image-5.png)
![alt text](image-6.png)
![alt text](image-7.png)
![alt text](image-8.png)
![alt text](image-9.png)

- https://aws.amazon.com/prescriptive-guidance/
- https://docs.aws.amazon.com/prescriptive-guidance/latest/load-testing/welcome.html?did=pg_card&trk=pg_card

![alt text](image-10.png)

![alt text](image-11.png)

- Route 53 healthcheck and metrics: what it is? Why do we need it? How it work?

![alt text](image-12.png)   

what it is? Why do we need it? How it work? AWS System Manager, Run Command


#### 1.3 Build and manage artifacts.

![alt text](image-13.png)

![alt text](image-14.png)

![alt text](image-15.png)

![alt text](image-16.png)

![alt text](image-17.png)
- Code deploy will use a load balancer with two target groups

![alt text](image-18.png)
- How do you add cross region actions in your pipeline?

#### 1.4 Implement deployment strategies for instance, container, and serverless environments.

- How, when, why to use difference deployment methods:
  - Blue/green
  - Canary
  - Immutable
  - Rolling
  - Rolling with additional batch
  - In Place
  - Linear
  - All-at-one

Relevant topic:
- https://nghethuatcoding.com/2019/05/06/cac-ki-su-grab-da-thiet-ke-he-thong-dan-hoi-su-dung-circuit-breaker-nhu-the-nao/

![alt text](image-19.png)
- What is the hooks of each deployment methods?
- Lambda versioning, alias

- Troubleshooting deployment issue
  - ingress egress of security group
  - vpc flow log???

**Tutorial:** https://docs.aws.amazon.com/codepipeline/latest/userguide/tutorials.html

