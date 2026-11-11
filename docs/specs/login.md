# Login page

Status: approved · Owner: Irina Lucuț

## Goal

Allow users and administrators to authenticate through a simulated client-side login in the browser to access the Task List and administrative controls, without a backend API.

## Out of scope

- Backend API communication and server-side authentication.
- User registration and account creation flow.
- Password reset or recovery links.
- Third-party OAuth authentication.
- Build tools or bundlers (Vite, Vue, Webpack).

## Behavior

- [ ] Given I open login.html, when it renders in the browser, then I see a styled Tailwind card with the title "Task List", inputs for Username and Password, helper text for demo credentials, and a "Log in" button.
- [ ] Given empty username or password fields, when I click "Log in", then I see an error message "Please fill in all fields" and login is prevented.
- [ ] Given invalid credentials, when I click "Log in", then I see an error message "Invalid username or password".
- [ ] Given user credentials (`user` / `password`), when I click "Log in", then session state is saved to localStorage with role `user` and a success notification is shown.
- [ ] Given admin credentials (`admin` / `admin123`), when I click "Log in", then session state is saved to localStorage with role `admin` and an admin success notification is shown.

## Done when

- [ ] every behavior line has been checked
