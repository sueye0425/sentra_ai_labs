# Netlify Forms Setup Guide

## How to Receive Form Submissions

After deploying your site to Netlify, you can access form submissions in multiple ways:

### 1. View Submissions in Netlify Dashboard

1. Go to [app.netlify.com](https://app.netlify.com)
2. Select your site
3. Click on **"Forms"** in the top navigation
4. Click on **"beta-waitlist"** form
5. You'll see all submissions with:
   - Email address
   - Submission date/time
   - IP address (optional, can be disabled for privacy)

### 2. Set Up Email Notifications

**Step-by-step instructions:**

1. Go to your Netlify dashboard → Select your site
2. Navigate to **Site settings** → **Forms** → **Form notifications**
3. Click **"Add notification"**
4. Select **"Email notifications"**
5. Configure:
   - **To email**: Your email address (e.g., yourname@example.com)
   - **From email**: Leave as default or customize
   - **Subject**: Customize (e.g., "New Cocoo Beta Signup")
   - **Form**: Select "beta-waitlist"
6. Click **"Save"**

**What you'll receive:**
- An email for each new submission
- Email includes:
  - User's email address
  - Submission timestamp
  - Form name
  - All form fields

### 3. Export Submissions as CSV

1. Go to **Forms** → **beta-waitlist**
2. Click **"Export CSV"** button
3. Download the CSV file with all submissions
4. Open in Excel, Google Sheets, or any spreadsheet app

### 4. Set Up Webhook Notifications (Advanced)

For automated workflows (e.g., add to Google Sheets, send to Slack):

1. Go to **Site settings** → **Forms** → **Form notifications**
2. Click **"Add notification"**
3. Select **"Webhook"**
4. Enter your webhook URL (from Zapier, Make.com, etc.)
5. Select form: **"beta-waitlist"**
6. Click **"Save"**

## What Information is Captured

Each submission includes:
- **Email address** (from the form field)
- **Submission timestamp**
- **IP address** (can be disabled in settings)
- **User agent** (browser/device info)
- **Form name**: "beta-waitlist"

## Form Configuration

The form is configured with:
- **Form name**: `beta-waitlist`
- **Spam protection**: Honeypot field (invisible to users)
- **Email validation**: Required field
- **Success/error messages**: Displayed to users after submission

## Testing the Form

1. Deploy your site to Netlify
2. Visit your live site
3. Fill out the form with a test email
4. Check your Netlify dashboard → Forms → beta-waitlist
5. You should see the submission appear within seconds

## Privacy & GDPR Compliance

- Netlify Forms are GDPR compliant
- You can disable IP address collection in form settings
- Users can request data deletion through you
- Consider adding a privacy policy link near the form

## Troubleshooting

**Form not working?**
- Make sure the form has `netlify` attribute (already added)
- Check that the form name matches: `beta-waitlist`
- Verify the site is deployed to Netlify (forms don't work locally)

**Not receiving emails?**
- Check spam/junk folder
- Verify email address in notification settings
- Check Netlify dashboard for any error messages
- Ensure form notifications are enabled

**Need to change the form?**
- Edit the form in `public/index.html`
- Redeploy to Netlify
- Existing submissions remain in the dashboard

