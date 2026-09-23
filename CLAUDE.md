# Claude Development Rules for South County Threadz Website

## Project Context
This is a **simple static one-page website** for South County Threadz, a curated clothing and fashion retail business. The website serves as a landing page with links to external selling platforms and social media.

## Critical Rules

### 1. Protect Client Information
- Never expose client contact details, email addresses, or personal information in code or commits
- Do not include credentials, API keys, or secrets in any files
- If access credentials are needed, store them in `.env.local` (not committed)

### 2. Never Commit Secrets or Credentials
- `.env.local` must be in `.gitignore`
- Do not hardcode API keys, tokens, or authentication details
- Do not add private/sensitive links or URLs to version control
- Verify all changes before committing

### 3. Do Not Invent Client Facts
- Use only information explicitly provided by the client or Sweet Creatives
- Do not guess or assume branding elements, copy, product descriptions, or business details
- Document all TBD items clearly in README.md
- Ask for clarification before making assumptions about design, content, or functionality

### 4. Do Not Expand Scope Without Instruction
- This is a **one-page landing page** only
- Do not add:
  - Multi-page navigation
  - Contact forms or email functionality
  - Shopping carts or payment processing
  - User accounts or authentication
  - CMS systems
  - Backend APIs
  - Databases or persistent storage
  - Firebase or third-party services
- Stick to the defined architecture: static HTML/CSS/JavaScript only
- Any scope changes require explicit client and Sweet Creatives approval

### 5. Do Not Perform Destructive Git Operations
- Do not use `git reset --hard`, `git clean -f`, `git push --force`, or similar destructive commands without explicit approval
- Always verify changes before committing
- Create clean, descriptive commits with proper attribution
- Do not amend or rebase published commits

### 6. Verify Changes Before Committing
- Review all file changes before staging
- Test the website in a browser to verify functionality
- Ensure accessibility (WCAG AA) compliance
- Verify mobile responsiveness
- Run validation tools if appropriate

### 7. Maintain Accessibility and Responsive Standards
- **Target:** WCAG AA accessibility compliance
- Semantic HTML structure
- Proper heading hierarchy
- Alt text for all images
- Color contrast compliance
- Mobile-first responsive design
- Touch-friendly interactive elements

## Placeholder Assets

A placeholder must be clearly documented for:
- **Logo:** Use a documented placeholder (e.g., comment with `<!-- PLACEHOLDER: Logo to be added -->`) until the final logo is available

Do not create or guess final branding assets during development.

## Stop Points

Before taking any of these actions, **stop and ask for explicit approval**:
- Creating a GitHub repository
- Committing changes to version control
- Pushing to any remote repository
- Deploying to production (Netlify or any hosting)
- Creating or modifying files outside this project directory
- Adding any third-party dependencies or services not listed here
- Making scope changes to the project

## Approved Tech Stack

- **HTML5** - semantic markup
- **CSS3** - responsive styling (no frameworks required)
- **Vanilla JavaScript** - minimal interactivity only
- **No build process required** - static site served as-is

Anything beyond this requires explicit approval.
