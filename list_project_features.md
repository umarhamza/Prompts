# List Project Features (User Perspective Only)

**Goal:** 
Generate a simple bulleted list of what users can actually DO in this project. No technical details.

**Input:** 
Project at: `{PROJECT_PATH}`

**Rules:**
- Only list user-facing features
- Use simple, non-technical language
- One feature per bullet point
- Start each bullet with an action verb
- No technical stack, architecture, or implementation details
- No developer/admin features unless they're user-facing

**Output Format:**
Save to `FEATURES_LIST.md`:

# Project Features

## What users can do:

- [Action verb] [what they can do]
- [Action verb] [what they can do]
- [Action verb] [what they can do]

**Examples of good feature descriptions:**
- Log in with email and password
- Upload and share photos
- Send messages to other users
- Search for products by name
- Add items to shopping cart
- Pay with credit card
- Track order status
- Leave reviews and ratings
- Create and edit profiles
- Get email notifications

**What to examine:**
- Routes/URLs (what pages exist)
- Forms (what users can submit)
- Buttons and actions (what users can click)
- API endpoints (what actions they trigger)
- Database models (what data users create)
- UI components (what interactions exist)

**What NOT to include:**
- "Uses React" (technical)
- "Has authentication middleware" (technical)
- "Connects to PostgreSQL database" (technical)
- "Admin can manage users" (unless it's user-facing)
- "Has CI/CD pipeline" (developer feature)
