# Student Task Tracker

Version: 1.0.0

A responsive task management application for recording student assignments, subjects, due dates, priority levels, and completion status.

## Features

- Create tasks with a title, subject, due date, and priority
- View all tasks
- Filter pending and completed tasks
- Mark tasks as complete
- Delete tasks
- Display progress statistics
- Persist tasks through a Supabase database
- Use a local browser preview when the API is not configured

## Technology

- HTML, CSS, and JavaScript
- Vercel serverless functions
- Supabase PostgreSQL
- GitHub for source control

## Project structure

- `index.html` — application page
- `style.css` — responsive interface
- `app.js` — client-side behavior
- `api/tasks.js` — backend API
- `supabase-schema.sql` — database table definition
- `docs/` — project plans and logs

## Local setup

1. Install Node.js.
2. Create a Supabase project.
3. Open the Supabase SQL Editor and run the contents of `supabase-schema.sql`.
4. Copy `.env.example` to `.env.local`.
5. Set `SUPABASE_URL` to the project URL.
6. Set `SUPABASE_SERVICE_ROLE_KEY` to the server-side service-role key.
7. Install dependencies with `npm install`.
8. Install or run Vercel CLI with `npx vercel dev`.
9. Open the local URL shown by Vercel.

Keep the service-role key private. Never place it in `app.js`, `index.html`, or any other frontend file. Do not commit `.env.local`.

## Deployment

1. Push the project to a GitHub repository.
2. Import the repository into Vercel.
3. Add `SUPABASE_URL` and `SUPABASE_SERVICE_ROLE_KEY` in the Vercel project environment variables.
4. Deploy the project.
5. Open the deployed URL and test task creation, listing, completion, and deletion.

## API

- `GET /api/tasks` — list tasks
- `POST /api/tasks` — create a task
- `PATCH /api/tasks?id=TASK_ID` — update completion status
- `DELETE /api/tasks?id=TASK_ID` — delete a task

## Version history

- `1.0.0` — initial project structure, responsive interface, task API, and Supabase integration.

## Testing checklist

- Add a task with a title.
- Add a task with a subject, due date, and priority.
- Confirm the task appears in the list.
- Mark the task complete and confirm the statistics change.
- Filter pending and completed tasks.
- Delete a task.
- Try an empty title and confirm it is rejected.
- Test the live deployment after every release.

## Limitations

This academic starter project does not include user accounts. The API uses a server-side Supabase service-role key and is intended for a controlled demonstration. Before public production use, add authentication, authorization, rate limiting, and stricter access controls.
