# Workers Compensation Information Portal

## Introduction

Welcome to the **Compensation Information Portal**, a web-based platform designed to display active and expired workers' compensation insurance policies for companies and organizations. Our portal allows public users to search for a company and instantly view its insurance policy status in real-time, ensuring compliance with regulatory standards.

You can explore the live version of the project using the following link:

[Live Demo](https://mudu-pay-insure.vercel.app/)

Read the detailed blog article summarizing the development process and key takeaways:

[Final Project Blog Article](https://#)

- **Author**: [Your Name](https://www.linkedin.com/in/josh-myles-a05689123)

---

## Installation

To set up the project locally, follow the steps below:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-repo-name/project-name.git
   cd project-name
   ```
2. **nstall dependencies: Ensure that Node.js and npm are installed. Then run:**:
   ```bash
   npm install
   ```
3. **Environment configuration: Create a .env file in the root directory and add the following environment variables:**:
   ```bash
    API_KEY=your_api_key_here
    DB_CONNECTION_STRING=your_database_url_here
   ```
4. **Run the development serve**:

   ```bash
   npm start

   The app should now be running at http://localhost:3000.
   ```

## Usage

This portal provides a seamless way for users to search for companies and view their workers' compensation insurance policies. The following are key features of the platform:

Search Companies: Users can search for companies using the company name or registration number.
Detailed Policy View: Clicking on search results will show detailed policy information including insurer, policy number, expiration date, and more.
Real-Time Notifications: Companies can receive alerts before a policy expires (premium feature).
Admin Dashboard: Allows administrators to manage policy records, monitor data trends, and visualize system metrics.

## APIS and methods

### API Routes:

- GET /api/policies: Retrieve a list of all policies.
- GET /api/policies/:companyId: Retrieve detailed policy information for a specific company.
- POST /api/notifications/subscribe: Subscribe to notifications for expiring policies.

### 3rd Party APIs:

- Insurance Data API: This provides real-time policy updates from insurance company databases.
- Notifications API: For sending expiration alerts via email/SMS to subscribed users.

## Data Modeling

We use a relational database with the following key entities:

1. Company: Stores information about each company (name, registration number, etc.).
2. Policy: Stores policy details (policy number, insurer, start date, expiration date, etc.).
3. User: Handles user authentication and access control.

## User Stories

1. Public User: As a public user, I want to search for companies by name or registration number and view their workers' compensation policy status.
2. Company Admin: As a company admin, I want to receive notifications before my workers' compensation policy expires.
3. System Admin: As a system administrator, I want to view and manage all policy records, track user activity, and generate reports.

## Architecture

This project follows a typical MVP (Minimum Viable Product) architecture. Below is the data flow from the frontend to the backend:

1. User Interaction: Users search for companies or policies.
2. Request Handling: The frontend sends requests to the backend via RESTful API routes.
3. Backend Processing: The backend (Node.js, Next.js) fetches data from the PostgreSQL database or third-party insurance APIs.
4. Response: The backend returns the requested data, which is then displayed on the frontend.

## Collaboration / Communication

Since this was a solo project, there wasn’t direct collaboration with peers. However, I did consult online communities for feedback and insights regarding integrating third-party APIs and ensuring scalability.

## Project Updates

The following adjustments were made during development:

1. Search Optimization: Enhanced full-text search capabilities to improve user experience.
2. Security Enhancements: Added stricter role-based access controls and audit logs to track administrator activity.

## Related Projects

[Teacher Effectiveness And Learner Achievement](https://telaschool.org)

## Licensing

This project is licensed under the MIT License – see the [LICENSE](https://opensource.org/license/mit) file for details.
