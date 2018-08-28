## Authorization


## Authorization

RBAC to restrict access to objects
- nodes,
- environments,
- roles,
- data bags,
- cookbooks, ...


## Authorization

- Only authorized user and/or chef-client requests to the Chef server are allowed.
- Access to objects on the Chef server is fine-grained, allowing access to be defined by object type e.g.
  - group, 
  - user, and 
  - organization. 


| Feature	   | Description   |
| -----------|:-------------:|
| Organization | Top-level entity for RBAC.|
| Group | To e.g. assign permissions that determine what types of tasks are available to members of that group who are authorized to perform them. |
| User | Any non-administrator human being who will manage data that is uploaded to the Chef server from a workstation|
| Client | Actor that has permission to access the Chef server. |


## Object Permissions

| Permission | Description   |
| -----------|:-------------:|
|Delete | Defines which users and groups may delete an object.|
|Grant   | Defines which users and groups may configure permissions on an object.|
|Read    | Define which users and groups may view the details of an object. |
|Update  | Defines which users and groups may edit the details of an object. |


## Global Permissions

| Permission | Description   |
| -----------|:-------------:|
| Create     | Define which users and groups may create the following server object types like cookbooks, data bags, environments, ... .|
| List	     | Define which users and groups may view the following server object types like cookbooks, data bags, environments, nodes, roles, and tags.|