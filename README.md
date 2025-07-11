
# Job Portal MVP

This document provides an overview of the Minimum Viable Product (MVP) for a new job portal platform. The goal is to create a simple and user-friendly platform that connects job seekers with employers, inspired by the core functionalities of sites like Indeed.

All the documentation for the MVP can be found in the `/mvp` directory.

## User Personas

We are focusing on two primary user personas for the MVP:

*   **Sarah (Job Seeker):** A recent graduate looking for her first full-time marketing job. She needs a simple, intuitive platform to search for relevant positions and apply easily.
*   **John (Employer):** The owner of a small tech startup who needs to hire a software developer. He needs an efficient way to post job openings and manage applications from qualified candidates.

For more details, see [mvp/user_personas.md](mvp/user_personas.md).

## MVP Features

The core features for the MVP are broken down by user type:

### Job Seeker Features

*   **Authentication:** Sign up, log in, and log out.
*   **Job Search:** Search by keyword and location, with basic filtering by job type (full-time, part-time, etc.).
*   **Job Viewing:** View a list of search results and detailed job descriptions.
*   **Job Application:** Apply for jobs using a simple form (Name, Email, Resume).

### Employer Features

*   **Authentication:** Sign up, log in, and log out.
*   **Job Posting:** Create new job postings with essential details (title, description, location, job type).
*   **Job Management:** View, edit, and delete their own job postings.
*   **Application Tracking:** View a list of applicants for each job and see their details.

For a complete list of requirements, see the [Product Requirements Document (PRD)](mvp/mvp.md).

## User Stories

Detailed user stories have been created to guide development, covering the features mentioned above. Each story includes clear acceptance criteria.

**Example User Story (Job Seeker):**
> As a job seeker, I want to search for jobs by keyword so that I can find relevant job openings.

For a complete list of user stories and their acceptance criteria, please see [mvp/user_stories.md](mvp/user_stories.md).

## Design and User Experience

The design of the platform will be clean, modern, and intuitive.

*   **UI Design:** The focus is on consistency, clarity, and simplicity. The site will be fully responsive. For wireframes and visual design guidelines, see [mvp/ui_design.md](mvp/ui_design.md).
*   **UX Design:** The user experience is designed to be user-centric, efficient, and engaging. The goal is to make the process of finding and applying for jobs (for seekers) and posting jobs and reviewing candidates (for employers) as seamless as possible. For user journey maps and UX principles, see [mvp/ux_design.md](mvp/ux_design.md).

## User Flow

The user flow for both job seekers and employers has been mapped out, from initial landing on the site to completing their primary goals.

Mermaid diagrams illustrating these flows are included in the [User Flow Document](mvp/user_flow.md).

## Non-Functional Requirements

*   **Performance:** The site must be fast and responsive.
*   **Security:** User data must be kept secure.
*   **Usability:** The platform should be intuitive and easy to use.
*   **Scalability:** The architecture should support a growing number of users.

## Future Enhancements (Out of MVP Scope)

The following features are planned for future releases but are not part of the MVP:

*   Advanced search filters (e.g., salary, experience level).
*   Company and job seeker profiles.
*   Email notifications.
*   Third-party login integration (Google, LinkedIn).
*   A more advanced application tracking system (ATS) features.
