Student Task Tracker

Version: 1.0.0  
Project Type: Capstone Project  
Developer: Melchor Aboc
FrontEnd: Kevin Jay Gracias

Project Description

Student Task Tracker is a web application designed to help students organize their assignments, subjects, deadlines, and priorities. It allows users to add tasks, view pending tasks, mark tasks as completed, and delete tasks. The application also displays task statistics to help students monitor their progress.

## Objectives

- Organize student assignments and deadlines.
- Track pending and completed tasks.
- Practice web application development.
- Implement a backend API connected to a database.
- Apply software maintenance, disaster recovery, and version control practices.
- Deploy the application online.

Technologies Used

- HTML
- CSS
- JavaScript
- Node.js
- Vercel
- Supabase PostgreSQL
- GitHub

Features

- Add tasks with titles and subjects.
- Set due dates and priority levels.
- View all tasks.
- Filter pending and completed tasks.
- Mark tasks as completed.
- Delete tasks.
- View task completion statistics.
- Responsive design for desktop and mobile devices.

Project Structure

- `index.html` — Main application page
- `style.css` — Application design and layout
- `app.js` — Frontend functionality
- `api/tasks.js` — Backend API
- `supabase-schema.sql` — Database table setup
- `docs/maintenance-plan.pdf` — Software Maintenance Plan
- `docs/disaster-recovery-plan.pdf` — Disaster Recovery Plan
- `docs/sprint-plan.pdf` — Sprint Plan
- `docs/team-charter.pdf` — Team Charter
- `docs/standup-log.pdf` — Standup Log

API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/api/tasks` | Retrieve tasks |
| POST | `/api/tasks` | Create a task |
| PATCH | `/api/tasks?id=TASK_ID` | Update task completion |
| DELETE | `/api/tasks?id=TASK_ID` | Delete a task |

Installation and Setup

1. Download or clone this repository.
2. Install Node.js.
3. Create a Supabase project.
4. Run the SQL commands in `supabase-schema.sql` using the Supabase SQL Editor.
5. Configure the required environment variables.
6. Install dependencies using `npm install`.
7. Run the application locally using `npx vercel dev`.
8. Open the local URL provided by Vercel.

Deployment

The application can be deployed using Vercel.

1. Import the GitHub repository into Vercel.
2. Configure `SUPABASE_URL` and `SUPABASE_SERVICE_ROLE_KEY` in the project's environment variables.
3. Deploy the application.
4. Test the website and API endpoints after deployment.

Keep database credentials private. Never upload secret keys to public frontend files or commit them to GitHub.

Software Maintenance

The application will be maintained through bug tracking, code updates, testing, dependency reviews, and GitHub version control. Issues will be documented and fixes will be tested before deployment. Previous working versions can be restored using Git history and Vercel deployment history.

Version History

Initial release of the Student Task Tracker.

Developer
Front End

Melchor Aboc
Bachelor of Science in Information Technology (BSIT)

Project Status

Developed as an academic Capstone Project covering deployment, software maintenance, disaster recovery, and Sprint 1 development.


