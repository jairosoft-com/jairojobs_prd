# User Stories for Job Portal MVP

## User Personas

*   **Job Seeker (Sarah)**
*   **Employer (John)**

## Job Seeker Stories (Sarah)

*   **US-1: Account Creation**
    *   As a job seeker, I want to create an account so that I can apply for jobs.
    *   **Acceptance Criteria (Given/When/Then):**
        *   **Scenario: Successful Registration**
        *   **Given** Sarah is a new user on the registration page,
        *   **When** she provides a valid name, a unique email, and a strong password, and clicks "Sign Up",
        *   **Then** her account is created, she is logged in, and redirected to her dashboard.
        *
        *   **Scenario: Email Already Exists**
        *   **Given** Sarah is on the registration page,
        *   **When** she enters an email address that already exists in the system,
        *   **Then** an error message "Email already in use. Please log in." is displayed.

*   **US-2: Account Login**
    *   As a job seeker, I want to log in to my account so that I can manage my applications.
    *   **Acceptance Criteria (Checklist):**
        *   [ ] The login form contains an email input field.
        *   [ ] The login form contains a password input field.
        *   [ ] A "Log In" button is present and clickable.
        *   [ ] Upon entering correct credentials and clicking "Log In", the user is redirected to their dashboard.
        *   [ ] Upon entering incorrect credentials, a "Invalid email or password." error message is displayed.
        *   [ ] The password field masks the input.

*   **US-3: Job Search by Keyword**
    *   As a job seeker, I want to search for jobs by keyword so that I can find relevant job openings.
    *   **Acceptance Criteria (Scenario-based):**
        *   **Scenario 1: Search with relevant results**
        *   **Given** Sarah is logged in and on the job search page,
        *   **When** she enters "Senior Product Manager" into the search bar and clicks "Search",
        *   **Then** the system displays a list of all job postings containing "Senior", "Product", or "Manager" in the title, ordered by relevance.
        *
        *   **Scenario 2: Search with no results**
        *   **Given** Sarah is on the job search page,
        *   **When** she enters a nonsensical keyword like "asdfghjkl" and clicks "Search",
        *   **Then** the system displays a message: "No jobs found. Try different or more general keywords."

## Employer Stories (John)

*   **US-4: Account Creation**
    *   As an employer, I want to create an account so that I can post job openings.
    *   **Acceptance Criteria (Given/When/Then):**
        *   **Scenario: Successful Employer Registration**
        *   **Given** John is a new employer on the employer registration page,
        *   **When** he provides a valid company name, a unique email, and a password, and clicks "Create Account",
        *   **Then** his employer account is created, he is logged in, and redirected to the employer dashboard.
        *
        *   **Scenario: Invalid Company Name**
        *   **Given** John is on the employer registration page,
        *   **When** he leaves the company name field blank and submits the form,
        *   **Then** an error message "Company name is required." is displayed next to the field.

*   **US-5: Post a Job**
    *   As an employer, I want to post a new job with all the necessary details so that I can attract qualified candidates.
    *   **Acceptance Criteria (Checklist):**
        *   [ ] The employer dashboard has a clearly visible "Post a New Job" button.
        *   [ ] The job creation form includes mandatory fields for: Job Title, Job Description, Location, and Job Type.
        *   [ ] The "Job Type" is a dropdown menu with options: "Full-time", "Part-time", "Contract", "Internship".
        *   [ ] Clicking "Post Job" without filling all mandatory fields displays specific error messages for each empty field.
        *   [ ] After successful submission, the job becomes publicly visible on the job board.
        *   [ ] The employer is redirected to the dashboard, where the new job appears at the top of their active postings list.

*   **US-6: View Applications**
    *   As an employer, I want to view a list of applicants for each of my job postings so that I can review the candidates.
    *   **Acceptance Criteria (Scenario-based):**
        *   **Scenario 1: Viewing a list of applications**
        *   **Given** John is logged into his employer dashboard and has a "Lead Developer" posting with 5 applications,
        *   **When** he clicks the "View Applicants" button for that posting,
        *   **Then** he is taken to a page that lists all 5 applicants.
        *   **And** each entry in the list shows the applicant's name, email, and the date they applied.
        *
        *   **Scenario 2: Viewing an empty application list**
        *   **Given** John has a newly created "Graphic Designer" job posting with 0 applications,
        *   **When** he clicks "View Applicants" for that posting,
        *   **Then** the system displays a message: "You have no applicants for this position yet."
