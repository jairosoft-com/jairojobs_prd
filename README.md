
# JairoJobs.com MVP

This document provides an overview of the Minimum Viable Product (MVP) for
[JairoJobs.com](https://jairojobs.com). The goal is to create a simple and
user-friendly platform that connects job seekers with employers, inspired by the
core functionalities of sites like [Indeed.com](https://www.indeed.com).

## 🗂️ Project Structure

This project follows a version-based organization structure:

```text
prd_jjcom/
├── README.md                    # This file - project overview
├── TODO_README_UPDATE.md        # TODO list for documentation updates
├── ai_docs/                     # AI documentation templates and formats
│   ├── acceptance_criteria_format.md
│   └── user_story_format.md
├── mvp1.0/                      # MVP version 1.0 documentation
│   ├── m1.0.1/                  # MVP 1.0.1 specifications
│   │   ├── product_spec.md      # Product Requirements Document
│   │   ├── model_spec.md        # Model specifications
│   │   ├── code_spec.md         # Code specifications
│   │   ├── user_personas.md     # User personas
│   │   ├── user_stories.md      # User stories with acceptance criteria
│   │   ├── user_flow.md         # User flow diagrams
│   │   ├── ui_design.md         # User interface design
│   │   └── ux_design.md         # User experience design
│   └── m1.0.2/                  # MVP 1.0.2 specifications
│       ├── product_spec.md
│       ├── model_spec.md
│       └── code_spec.md
├── v1.0/                        # Version 1.0 documentation
│   ├── v1.0.1/
│   │   ├── product_spec.md
│   │   ├── model_spec.md
│   │   └── code_spec.md
│   └── v1.0.2/
│       ├── product_spec.md
│       ├── model_spec.md
│       └── code_spec.md
└── v2.0/                        # Version 2.0 documentation
    ├── v2.0.1/
    │   ├── product_spec.md
    │   ├── model_spec.md
    │   └── code_spec.md
    └── v2.0.2/
        ├── product_spec.md
        ├── model_spec.md
        └── code_spec.md
```

### Directory Purpose

- **`mvp1.0/`**: Contains the Minimum Viable Product documentation and specifications
- **`v1.0/`**: Contains version 1.0 documentation for future releases
- **`v2.0/`**: Contains version 2.0 documentation for advanced features
- **`ai_docs/`**: Contains templates and formats for AI-generated documentation

## 🚀 Getting Started

### Quick Reference

| Document Type | Location |
|---------------|----------|
| Product Requirements | `mvp1.0/m1.0.1/product_spec.md` |
| User Stories | `mvp1.0/m1.0.1/user_stories.md` |
| User Personas | `mvp1.0/m1.0.1/user_personas.md` |
| User Flow Diagrams | `mvp1.0/m1.0.1/user_flow.md` |
| UI Design | `mvp1.0/m1.0.1/ui_design.md` |
| UX Design | `mvp1.0/m1.0.1/ux_design.md` |
| Model Specifications | `mvp1.0/m1.0.1/model_spec.md` |
| Code Specifications | `mvp1.0/m1.0.1/code_spec.md` |

### Navigation Tips

1. **For Product Managers**: Start with `product_spec.md` and `user_stories.md`
2. **For Designers**: Focus on `ui_design.md` and `ux_design.md`
3. **For Developers**: Review `model_spec.md` and `code_spec.md`
4. **For Stakeholders**: Begin with `user_personas.md` and `user_flow.md`

## 💻 Development Setup

### Prerequisites

- [Visual Studio Code](https://code.visualstudio.com/) (recommended)
- Git for version control
- Basic knowledge of Markdown syntax

### Required VSCode Extensions

#### Markdown Support

- **Markdown All in One** - All-in-one markdown plugin
  - Install: `Ctrl+Shift+X` → Search "Markdown All in One"
  - Features: Auto-completion, keyboard shortcuts, list editing
- **Markdown Preview Enhanced** - Enhanced markdown preview
  - Install: `Ctrl+Shift+X` → Search "Markdown Preview Enhanced"
  - Features: Live preview, math equations, diagrams
- **markdownlint** - Markdown linting and style checking
  - Install: `Ctrl+Shift+X` → Search "markdownlint"
  - Features: Style checking, error highlighting

#### Mermaid Diagram Support

- **Mermaid Preview** - Preview mermaid diagrams
  - Install: `Ctrl+Shift+X` → Search "Mermaid Preview"
  - Features: Live preview of mermaid diagrams
- **Mermaid Markdown Syntax Highlighting** - Syntax highlighting for mermaid
  - Install: `Ctrl+Shift+X` → Search "Mermaid Markdown Syntax Highlighting"
  - Features: Proper syntax highlighting in markdown files

### Configuration Recommendations

Add to your VSCode settings.json:

```json
{
  "markdown.preview.breaks": true,
  "markdown.extension.toc.levels": "1..6",
  "markdown.extension.toc.orderedList": false,
  "markdownlint.config": {
    "MD013": {
      "line_length": 80,
      "code_blocks": false,
      "tables": false
    }
  }
}
```

## 👥 User Personas

We are focusing on two primary user personas for the MVP:

- **Sarah (Job Seeker):** A recent graduate looking for her first full-time
  marketing job. She needs a simple, intuitive platform to search for relevant
  positions and apply easily.
- **John (Employer):** The owner of a small tech startup who needs to hire a
  software developer. He needs an efficient way to post job openings and manage
  applications from qualified candidates.

For more details, see
[mvp1.0/m1.0.1/user_personas.md](mvp1.0/m1.0.1/user_personas.md).

## 🎯 MVP Features

The core features for the MVP are broken down by user type:

### Job Seeker Features

- **Authentication:** Sign up, log in, and log out.
- **Job Search:** Search by keyword and location, with basic filtering by job
  type (full-time, part-time, etc.).
- **Job Viewing:** View a list of search results and detailed job descriptions.
- **Job Application:** Apply for jobs using a simple form (Name, Email, Resume).

### Employer Features

- **Authentication:** Sign up, log in, and log out.
- **Job Posting:** Create new job postings with essential details (title,
  description, location, job type).
- **Job Management:** View, edit, and delete their own job postings.
- **Application Tracking:** View a list of applicants for each job and see their
  details.

For a complete list of requirements, see the
[Product Requirements Document (PRD)](mvp1.0/m1.0.1/product_spec.md).

## 📖 User Stories

Detailed user stories have been created to guide development, covering the
features mentioned above. Each story includes clear acceptance criteria.

**Example User Story (Job Seeker):**
> As a job seeker, I want to search for jobs by keyword so that I can find
> relevant job openings.

For a complete list of user stories and their acceptance criteria, please see
[mvp1.0/m1.0.1/user_stories.md](mvp1.0/m1.0.1/user_stories.md).

## 🎨 Design and User Experience

The design of the platform will be clean, modern, and intuitive.

- **UI Design:** The focus is on consistency, clarity, and simplicity. The site
  will be fully responsive. For wireframes and visual design guidelines, see
  [mvp1.0/m1.0.1/ui_design.md](mvp1.0/m1.0.1/ui_design.md).
- **UX Design:** The user experience is designed to be user-centric, efficient,
  and engaging. The goal is to make the process of finding and applying for jobs
  (for seekers) and posting jobs and reviewing candidates (for employers) as
  seamless as possible. For user journey maps and UX principles, see
  [mvp1.0/m1.0.1/ux_design.md](mvp1.0/m1.0.1/ux_design.md).

## 🔄 User Flow

The user flow for both job seekers and employers has been mapped out, from
initial landing on the site to completing their primary goals.

Mermaid diagrams illustrating these flows are included in the
[User Flow Document](mvp1.0/m1.0.1/user_flow.md).

## ⚡ Non-Functional Requirements

- **Performance:** The site must be fast and responsive.
- **Security:** User data must be kept secure.
- **Usability:** The platform should be intuitive and easy to use.
- **Scalability:** The architecture should support a growing number of users.

## 🚀 Future Enhancements (Out of MVP Scope)

The following features are planned for future releases but are not part of the
MVP:

- Advanced search filters (e.g., salary, experience level).
- Company and job seeker profiles.
- Email notifications.
- Third-party login integration (Google, LinkedIn).
- A more advanced application tracking system (ATS) features.

## 🤝 Contributing

### Documentation Standards

- Follow the 80-character line limit for markdown files
- Use proper heading hierarchy (H1 → H2 → H3)
- Include descriptive commit messages
- Test all internal links before committing

### Git Workflow

1. Create a feature branch for documentation updates
2. Make changes following the established format
3. Test markdown rendering and mermaid diagrams
4. Submit a pull request with clear description
5. Ensure all links are working correctly

### Troubleshooting

**Common Issues:**

- **Mermaid diagrams not rendering**: Ensure Mermaid Preview extension is installed
- **Markdown linting errors**: Check line length and formatting
- **Broken links**: Verify file paths after directory changes

**Getting Help:**

- Check the [ai_docs/](ai_docs/) directory for formatting templates
- Review existing documentation for style consistency
- Use VSCode's built-in markdown preview for testing
