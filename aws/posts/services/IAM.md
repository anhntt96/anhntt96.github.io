## AWS Identity and Access Management (IAM)

### Tutorial
[IAM crashcourse Viet Tran](https://www.youtube.com/watch?v=RVDwsmyFA-Q&list=PL4NoNM0L1m72rjn5s7VzKnaqEK7UTpeGa)


### Note

Good things to do:
- Add MFA to root user
- Create account alias
- Do not use root user for daily basis work. Create a user with needed permission.
- Create group users and attach policies to group. Add users to group. This will help manage permissions of multiple users.

#### Policy
3 types:
- AWS Managed policy
- Customer managed policy
- Inline policy (not recommend)

Tools:
- [IAM Policy Simulator](https://policysim.aws.amazon.com/home/index.jsp)
- [AWS Policy Generator](https://awspolicygen.s3.amazonaws.com/policygen.html)

#### Roles
- Assume Role
  - administrator must create the role in the account you want to switch to, and then grant it permissions to perform the task you want
  - administrator provides you with the account ID or alias and the role name to use
  - Click your user name in the navigation bar, then select Switch Role. Enter the account and role information provided by your administrator. You immediately begin using the permissions associated with the new role

#### Identity Federation / Federating
- SAML, OpenID

### Questions
1. How many target that 1 rule can handle?
   - [You can define up to five targets for each rule](https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-targets.html)
2. Is it run 1 by 1 or parallel?
   - [run in parallel](https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-rules.html)