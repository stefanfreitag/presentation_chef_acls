## Authorization


## Authorization

Role based access control to restrict access to objects like

- nodes,
- environments,
- roles,
- data bags,
- cookbooks, 
- ...


## Authorization

- Only authorized user and/or chef-client requests to the Chef server are allowed.
- Fine-grained access levels, allowing access to be defined by object type e.g.
  - group,
  - user, and
  - organization.


| Feature	   | Description   |
| -----------|:-------------:|
| Organization | Top-level entity for RBAC.|
| Group | List of users. |
| User | Any non-administrator human being. |
| Client | Actor that has permission to access the Chef server. |


## Object Permissions

| Permission | Description   |
| -----------|:-------------:|
|Delete | Delete an object.|
|Grant   | Configure permissions on an object.|
|Read    | View the details of an object. |
|Update  | Edit the details of an object. |


## Global Permissions

| Permission | Description   |
| -----------|:-------------:|
| Create     | Create server object types like cookbooks, data bags, environments, ... .|
| List	     | View server object types like cookbooks, data bags, environments, nodes, ... .|