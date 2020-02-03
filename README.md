# project-management-spec
This is a spec document for the project management tool that is my base project for each new language/platform/framework/tool I learn.

---

# Basic Project Layout
- Home page
- Login pages

# Login Sections
- Projects
- Clients
- Tasks
- Servers
- Comments

## User Section
- Signup
- Login
- Forgot Password
- Reset Password
#### User Fields
- ID
- email
- password

## Project Section
- Project List
- Project Create
- Project Edit
- Project Delete
#### Project Fields
- ID
- Name
- Client (FK)
- Description
- Comments (FK)
- Private Info (passwords, logins, etc.)
- Files (File Uploads)
- Server (FK)
- User (FK)
- Status (FK)

## Client Section
- Client List
- Client Create
- Client Edit
- Client Delete
#### Client Fields
- ID
- Name
- Contact Name
- Contact Email
- Contact Phone
- Comments (FK)
- User (FK)
- Status (FK)

## Task Section
- Task List
- Task Create
- Task Edit
- Task Delete
#### Task Fields
- ID
- Name
- Project (FK)
- Description
- Start Date
- Due Date
- Comments(FK)
- User (FK)
- Status (FK)

## Server Section
- Server List
- Server Create
- Server Edit
- Server Delete
#### Server Fields
- ID
- Hostname
- Platform (DO, AWS, etc.)
- Control Panel (CPanel, RunCloud, None, etc.)
- Public IP
- Monthly Cost
- Size (CPUs, RAM, Disk Space, etc.)
- User (FK)
- Status (FK)

## Additional Related Models
#### Comment Model
- ID
- User
- Text

#### Status Model
- ID
- Name
- Slug
