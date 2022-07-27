# Code 401 - Class 33

## `<Login />` and `<Auth />`

### [What is Role Based Access Control (RBAC)?](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more)

**What is Role Based Access Control (RBAC)?**

- A practice of retricting network access based on someone's role within an organization

**Share an example of RBAC including all possible CRUD operations and correlating roles.**

- An example RBAC hierarchy might be:

  - **READ** access: Can access a resource, but cannot modify, add, or delete. Roles might include a coordinator, customer service rep, sales rep
  - **CREATE** access: Can add a resource if needed
  - **UPDATE** access: Can modify an existing record. A project manager or account manager might require create and/or read access
  - **DELETE** access: Can delete an existing record. This might be an admin role

**What are the Benefits of RBAC?**

### Compare and Contrast the following two Libraries and the following questions. Yes, they are similarly named

[react-cookie library](https://www.npmjs.com/package/react-cookie)

[react-cookies component](https://www.npmjs.com/package/react-cookies)

**Describe some `react-cookie` features.**

- This allows the loading and saving of cookies within an application
- `withCookies(Component)` will give access to your cookies anywhere
- `set(name, value, [options])` will set a cookie value
- `remove(name, [options])` will remove a cookie

**Describe some `react-cookies` features.**

- Similar to `react-cookie`, this allows you to load and save cookies within React
- `.loadAll()` loads all available cookies, and returns an `object` containing all cookies
- `.save(name, value, [options])` allows you to set a cookie
- `.plugToRequest(req, res): unplug()` loads the user cookies, allowing you to do server-rendering and match the same results. Sends new cookies back to the user.

**Which library would you prefer would you prefer? Why?**

- I might prefer `react-cookie` because it works with React hooks, so implementation might be a bit easier

[Back to Home](../README.md)
