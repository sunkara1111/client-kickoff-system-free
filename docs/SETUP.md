# Setup Guide — Client Kickoff System

Complete setup instructions to get the Client Kickoff System running on your local device or in Notion.

**Created by Dineshgopi Sunkara** · Senior Controls Engineer · Automation Engineer

## Table of Contents

1. [Quick Start](#quick-start)
2. [Option A: Use in Notion](#option-a-use-in-notion)
3. [Option B: Use Locally / Other Apps](#option-b-use-locally--other-apps)
4. [Option C: View as Static Site](#option-c-view-as-static-site)
5. [Customization](#customization)
6. [Troubleshooting](#troubleshooting)

---

## Quick Start

**Goal:** Get from download to first client pipeline entry in 20 minutes.

### Prerequisites

- Text editor or notes app (Notion, Google Docs, Obsidian, Apple Notes, VS Code, etc.)
- Optional: AI tool access (ChatGPT, Claude, etc.) for prompts
- Optional: Web browser (to view the landing page)

### What's Included

```
Client-Kickoff-System.zip
├── Client-Kickoff-System.md      # Main system guide (paste into Notion/Docs)
├── LICENSE-Personal-Use.txt      # License terms
├── COPYRIGHT.md                   # Copyright information
├── PATENT_NOTICE.md              # Patent status (none claimed)
└── docs/
    └── SETUP.md                  # This file
```

The public landing page lives on GitHub Pages: https://sunkara1111.github.io/client-kickoff-system-free/

---

## Option A: Use in Notion

**Recommended for most freelancers.** Notion's database features make the Client Pipeline especially powerful.

### Step 1: Download and Extract

1. Download `Client-Kickoff-System.zip`
2. Extract the ZIP file to a folder on your device
3. Open `Client-Kickoff-System.md` in a text editor

### Step 2: Set Up Notion Workspace

1. **Create Main Page**
   - In Notion, create a new page titled **Client Kickoff System**
   - Choose a workspace (personal or team)

2. **Create Client Pipeline Database**
   - Inside your main page, type `/database` and create a new database
   - Title it **Client Pipeline**
   - Add these properties (columns):
     - `Client Name` (Title) — default, already exists
     - `Contact Name` (Text)
     - `Email` (Email)
     - `Channel` (Select) — Options: Email, Instagram DM, LinkedIn, Referral, Website Form, Other
     - `Service Type` (Select) — Options: Writing, Design, Dev, Consulting, Coaching, Other
     - `Status` (Select) — Options: Inquiry, Qualified, Intake Received, Scope Sent, Payment Pending, Kickoff Scheduled, Active, On Hold, Completed, Not a Fit, Ghosted
     - `Inquiry Date` (Date)
     - `Kickoff Date` (Date)
     - `Deposit / Amount` (Number, formatted as currency)
     - `Paid?` (Checkbox)
     - `Priority` (Select) — Options: Hot, Warm, Cold
     - `Fit Score` (Select) — Options: Strong Fit, Maybe, Weak Fit
     - `Next Action` (Text)
     - `Next Action Due` (Date)
     - `Notes` (Text)
     - `Client Page` (URL or Relation)

3. **Add Pipeline Views**
   - Create these helpful views:
     - **Kanban**: Board grouped by Status
     - **Today**: Filter where Next Action Due is today/overdue
     - **Active**: Filter where Status = Active
     - **Unpaid**: Filter where Paid? = unchecked AND Status is Payment Pending or later

### Step 3: Add Templates

1. **Create Templates Folder**
   - Inside your main Client Kickoff System page, create a subpage called **Templates**

2. **Copy Template Pages**
   - From `Client-Kickoff-System.md`, copy each template section (C1–C7) into separate Notion pages:
     - Welcome Packet
     - Client Intake
     - Scope of Work
     - Kickoff Call Agenda
     - Revision Tracker
     - Invoice & Payment Checklist
     - Project Handoff / Close-out

3. **Customize Placeholders**
   - Replace these placeholders in each template:
     - `[Your Name / Studio]` → Your name
     - `[Email]` → Your email
     - `[Website]` → Your website
     - `[Timezone]` → Your timezone
     - Payment links, calendar links, etc.

### Step 4: Add AI Prompt Engine

1. Create a page called **AI Prompt Engine**
2. Copy Section D from `Client-Kickoff-System.md`
3. Paste all 8 prompts
4. Customize the prompt placeholders with your defaults

### Step 5: Test Run

1. Add the sample client "Acme Brand Refresh" to your Pipeline (optional)
2. Create a test inquiry and walk through Inquiry → Qualified
3. Verify your email templates work

**You're ready!** Next real inquiry: add to Pipeline → use Prompt 1 → go.

### Notion-Specific Tips

- **Duplicate Templates**: When a client converts, duplicate the relevant template pages into their workspace
- **Database Relations**: Link Client Pipeline rows to their template pages using the Client Page field
- **Automation**: Use Notion's built-in buttons or automations for recurring actions
- **Mobile**: Notion mobile app works well for quick status updates

---

## Option B: Use Locally / Other Apps

**For Google Docs, Obsidian, Craft, Apple Notes, or simple file systems.**

### Step 1: Extract Files

1. Download and extract `Client-Kickoff-System.zip`
2. Open `Client-Kickoff-System.md` in your preferred app

### Step 2: Set Up Client Pipeline

**Spreadsheet Option** (Google Sheets, Excel, Airtable):
1. Create a new spreadsheet called "Client Pipeline"
2. Add column headers from Section B of the guide
3. Set up status dropdowns for easy filtering

**Markdown/Document Option** (Obsidian, Craft):
1. Create a folder called "Client Kickoff System"
2. Create individual markdown files for each template
3. Use your app's tagging or linking features for the pipeline

### Step 3: Customize Templates

1. Create separate files/pages for each template (C1–C7)
2. Replace all placeholder text with your details
3. Save in an easily accessible location

### Step 4: Add Prompts

1. Create a "Prompts" document or note
2. Copy all 8 AI prompts from Section D
3. Keep it handy for quick copy-paste to ChatGPT/Claude

### Step 5: First Use

1. Add your first inquiry to the pipeline
2. Copy Prompt 1, fill in the details, and generate your reply
3. Follow the workflow from there

---

## Option C: View as Static Site

**To view the landing page locally** (or use the live site at https://sunkara1111.github.io/client-kickoff-system-free/).

### Simple Method (No Server)

1. Visit the live site: https://sunkara1111.github.io/client-kickoff-system-free/
2. Or clone this repository and open `index.html` in your browser

### With a Local Server

If you need to test locally with proper server headers:

**Using Python:**
```bash
# Navigate to the extracted folder
cd /path/to/Client-Kickoff-System

# Python 3
python3 -m http.server 8000

# Open browser to http://localhost:8000
```

**Using Node.js (npx):**
```bash
npx http-server -p 8000
```

**Using VS Code:**
1. Install "Live Server" extension
2. Right-click `index.html`
3. Select "Open with Live Server"

---

## Customization

### Identity and Branding

Replace these throughout all files:

- **Name**: Replace placeholder names with yours
- **Title/Role**: Add your professional identity
- **Contact**: Add your email, website, social links
- **Timezone**: Update to your timezone
- **Services**: Customize service types for your niche

### AI Prompts

Edit prompts to match your:
- Writing voice and tone
- Service complexity
- Client sophistication level
- Typical project scope

### Templates

Adapt templates for:
- Your specific deliverables
- Payment terms (deposit %, invoicing schedule)
- Revision policies
- Industry-specific questions

### Status Flow

Modify Pipeline statuses if you:
- Skip certain steps (e.g., no deposits for retainer clients)
- Add custom stages (e.g., "Under Contract Review")
- Have different closure states

---

## Troubleshooting

### Notion Import Issues

**Problem**: Formatting looks wrong when pasting  
**Solution**: 
- Use Notion's "Paste and Match Style" (Cmd/Ctrl + Shift + V)
- Or paste into a code block first, then format

**Problem**: Database properties not showing correctly  
**Solution**: 
- Delete and re-add the property with the exact type
- Check that Select options are created before adding data

### AI Prompt Issues

**Problem**: AI responses feel too formal/casual  
**Solution**: Add "Tone: [your preference]" to each prompt's instructions

**Problem**: Prompts generate too much text  
**Solution**: Add word count limits (e.g., "120-150 words") to each prompt

### File Organization

**Problem**: Can't find templates when needed  
**Solution**: 
- Use consistent naming (e.g., "TEMPLATE - Welcome Packet")
- Star/bookmark your most-used templates
- Keep a quick-reference checklist

### Pipeline Management

**Problem**: Statuses getting messy  
**Solution**: 
- Review and update statuses daily
- Move stale inquiries to "Ghosted" after 2 follow-ups
- Archive completed projects monthly

---

## Getting Help

- **Documentation**: Read the full guide in `Client-Kickoff-System.md`
- **Issues**: Open an issue on GitHub
- **Repository**: https://github.com/sunkara1111/client-kickoff-system-free

---

## What's Next?

Once you're set up:

1. ✅ Test with a sample/past client to verify the flow
2. ✅ Add real inquiry and follow the 24-hour kickoff path
3. ✅ Refine prompts and templates based on real use
4. ✅ Add optional automations (Zapier, Notion buttons, etc.)

---

## Quick Reference: 24-Hour Kickoff Path

| Time | Action | Status | Tools |
|------|--------|--------|-------|
| Hour 0 | Inquiry arrives | Inquiry | Pipeline + Prompt 1 |
| Hour 1-2 | Client engaged | Qualified | Prompt 2-3 + Intake |
| Hour 4-6 | Intake returned | Intake Received | Scope template + Prompt 4 |
| Hour 6-8 | Scope approved | Scope Sent → Payment Pending | Invoice checklist |
| Hour 8-12 | Payment received | Payment Pending → Kickoff Scheduled | Prompt 5 |
| Hour 12-24 | Kickoff call booked | Kickoff Scheduled | Kickoff agenda |

*Requires responsive client. Your side should never be the bottleneck.*

---

**Ready to streamline your client onboarding?**

Follow Option A, B, or C above, and you'll have your first client moving through the system within 24 hours.

---

© 2026 Dineshgopi Sunkara · Senior Controls Engineer · Automation Engineer  
Licensed under Personal Use License — See `LICENSE-Personal-Use.txt`
