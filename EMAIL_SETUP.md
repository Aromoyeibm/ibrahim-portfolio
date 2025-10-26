# EmailJS Setup Guide for Contact Form

This guide will help you set up EmailJS to make your contact form work.

## Step 1: Create EmailJS Account

1. Go to https://www.emailjs.com
2. Click "Sign Up" (it's free)
3. Create your account using your email

## Step 2: Add Email Service

1. In your EmailJS dashboard, go to **Email Services**
2. Click **Add New Service**
3. Select **Gmail** (or your preferred email provider)
4. Follow the authorization steps to connect your email
5. Note down your **Service ID** (looks like: `service_xxxxxxx`)

## Step 3: Create Email Template

1. Go to **Email Templates** in your dashboard
2. Click **Create New Template**
3. Use the following template:

### Template Subject:
```
New Contact Form Message: {{subject}}
```

### Template Content (HTML):
```html
<!DOCTYPE html>
<html>
<body>
    <h2>New Contact Form Message</h2>
    
    <p><strong>From:</strong> {{from_name}} &lt;{{from_email}}&gt;</p>
    <p><strong>Subject:</strong> {{subject}}</p>
    
    <h3>Message:</h3>
    <p>{{message}}</p>
    
    <hr>
    <p style="color: #999; font-size: 12px;">This message was sent from your portfolio contact form.</p>
</body>
</html>
```

### Template Settings:
- **Template Name**: Contact Form
- **To Email**: Enter your email address (e.g., ibrahim.aromoye@postgrad.manchester.ac.uk)
- **Reply To**: {{from_email}}
- **To Name**: Your Name

4. Click **Save**
5. Note down your **Template ID** (looks like: `template_xxxxxxx`)

## Step 4: Get Your Public Key

1. Go to **Account** → **General**
2. Find your **Public Key** (looks like: `your_public_key_here`)
3. Copy it

## Step 5: Update script.js

Open `script.js` and find these lines (around line 93 and 111):

### Line 93 - Replace with your Public Key:
```javascript
emailjs.init("your_actual_public_key_here");
```

### Line 111 - Replace with your Service ID and Template ID:
```javascript
emailjs.send('your_service_id', 'your_template_id', {
    from_name: data.name,
    from_email: data.email,
    subject: data.subject,
    message: data.message,
    to_email: 'ibrahim.aromoye@postgrad.manchester.ac.uk'
})
```

### Example:
```javascript
// Line 93
emailjs.init("ABC123XYZ");

// Line 111
emailjs.send('service_abc123', 'template_xyz789', {
    from_name: data.name,
    from_email: data.email,
    subject: data.subject,
    message: data.message,
    to_email: 'ibrahim.aromoye@postgrad.manchester.ac.uk'
})
```

## Step 6: Test Your Form

1. Open your portfolio in a browser
2. Scroll to the contact form
3. Fill out the form with test data
4. Submit the form
5. Check your email inbox for the message

## Troubleshooting

### Form not sending?
- Check browser console (F12) for errors
- Verify all IDs are correct in script.js
- Make sure your EmailJS account is verified

### Emails going to spam?
- Check your spam/junk folder
- The emails come from EmailJS servers, not your domain

### Need help?
Visit EmailJS documentation: https://www.emailjs.com/docs/

---

**Important**: Keep your Public Key, Service ID, and Template ID secure. Don't commit sensitive credentials to public repositories.

