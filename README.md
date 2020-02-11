# project-management-spec
This is a spec document for the project management tool that is my base project for each new language or framework or tool I learn.

The focus will not be on HTML or CSS. I will attempt to use the same static template for all of the projects I use to make learning the important pieces of the new language the focus of this exercise. I will consider this complete when all models are implemented as described. This will be a basis for learning a new language by creating and debugging the most common build scenarios. The auth pieces of this project are the last priority before testing. Auth may turn out to take significantly more time than it provides in value for some projects.

I plan to include a Vagrantfile with each project to more easily facilitate development on each project in the future.

Tests are secondary but will definitely solidify my confidence with any language I take a stab at.

The intent is to spend somewhere in the ballpark of 40 hours for each project, giving enough time to become familiar with most major concepts and significant debugging while keeping the project managable and not overwhelming.

[Project HTML Base](https://github.com/codescribblr/project-manager-html)

---

# Basic Project Layout
- Home page
- Login pages

# Login Sections
- Projects
- Clients
- Tasks
- Servers

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
- Notes (FK)
- Private Info (passwords, logins, etc.)
- Files (File Uploads)
- Server (FK)
- User (FK)
- Status

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
- Notes (FK)
- User (FK)
- Status

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
- Notes (FK)
- User (FK)
- Status

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
- Notes (FK)
- User (FK)

## Additional Related Models
#### Comment Model - One Model for each Major Model except Users
- ID
- User
- Text
