## Role-Based Access Control (RBAC)

DEFINITION:
Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

Access can be based on several factors, such as authority, responsibility, and job competency.

Some of the designations in an RBAC tool can include:
- Management role scope – it limits what objects the role group is allowed to manage.
- Management role – these are the types of tasks that can be performed by a specific role group.

options for user access may include:
- Primary – the primary contact for a specific account or role.
- Technical – assigned to users that perform technical tasks.
- Administrative – access for users that perform administrative tasks.

### BENEFITS OF RBAC
- Reducing administrative work and IT support.
- Maximizing operational efficiency.
- Improving compliance.

### react-cookie
Cookies are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites that the users browse and use it to verify them.

Setting up cookies:
```
const [cookies, setCookie, removeCookie] = useCookies(['cookie-name']);
```
Parameters:
- Cookies: Javascript object with all of the user’s cookies.
- setCookie: Function to set the cookies.
- removeCookie: Function to remove the cookies.