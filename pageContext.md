You can access pageContext by `this.context.pageContext` on root/main file `webpart` directory in spfx project.

this.context.pageContext.user
----
- displayName
- email
- isAnonymousGuestUser
- isExternalGuestUser
- loginName
- preferUserTimeZone

this.context.pageContext.web
----
- absoluteUrl
- description
- id
- isAppWeb
- language
- logoUrl
- permissions
- serverRelativeUrl
- templateName
- title

Reference
----
https://docs.microsoft.com/en-us/javascript/api/sp-page-context/pagecontext?view=sp-typescript-latest
