##  Authentication


##  Authentication

- Communication with Chef server must be authenticated
- Ensures that the Chef server responds only to requests made by trusted users
- Only authenticated requests will be authorized
- Implementation uses public key encryption


##  Authentication

- When a node and/or a workstation is configured to run the chef-client, public and private keys are created
- The public key is stored on the Chef server
- The private key is returned to the user for safe keeping
- The private key is a .pem file located in the .chef directory or in /etc/chef.


## Knife

- RSA public key-pairs are used to authenticate knife with the Chef server
- Ensures that 
  - each instance of knife is properly registered with the Chef server and
  - that only trusted users can make changes to the data.



## Authorization
- RBAC to restrict access to objects—nodes, environments, roles, data bags, cookbooks, ...
- Only authorized user and/or chef-client requests to the Chef server are allowed.
- Access to objects on the Chef server is fine-grained, allowing access to be defined by object type, object, group, user, and organization. 
- The Chef server uses permissions to define how a user may interact with an object, after they have been authorized to do so.


## Object Permissions
| Permission | Description   |
| -----------|:-------------:|
| Delete | Defines which users and groups may delete an object.|
|Grant   | Defines which users and groups may configure permissions on an object.|
|Read    | Define which users and groups may view the details of an object. |
|Update  | Defines which users and groups may edit the details of an object. |

# Links

https://docs.chef.io/auth.html