# Writers Grove URL Structure

## Main Domain Routes

### Public/Marketing

- `writersgrove.net` → Landing/marketing page

### Authentication

- `writersgrove.net/signin` → Sign in
- `writersgrove.net/signup` → Sign up
- `writersgrove.net/logout` → Logout

### Dashboard (Writing/Management)

- `writersgrove.net/dashboard` → User's writing workspace (default landing for writers after login)

### Library (Reading)

- `writersgrove.net/library` → Browse all public works (default landing for readers after login)
- `writersgrove.net/library/username` → Specific author's public page

## Subdomain Routes (Premium Users Only)

- `username.writersgrove.net` → Maps to `writersgrove.net/library/username`
  - Provides custom subdomain for premium users
  - Allows users to add their own advertisements (e.g., Google AdWords)
  - When logged in as the subdomain owner, shows the same public library view
  - Dashboard access still requires navigating to main `writersgrove.net` domain

## Reserved Subdomains

- `beta.writersgrove.net` → Main page
- Additional reserved: `www`, `api`, `admin`, `app`, `help`, `support`, `docs`, `status`, etc.

## User Types

- **Writers** → Default landing: `/dashboard`
- **Readers** → Default landing: `/library`
- Users can be both, preference set at signup (can toggle between views)
