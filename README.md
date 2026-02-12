# Clever Cloud Morocco Website

## 🚀 Setup Instructions

### 1. EmailJS Configuration

To enable the contact form, you need to set up EmailJS:

#### Step 1: Create config.js
```bash
cp config.example.js config.js
```

#### Step 2: Get EmailJS Credentials

1. Sign up at [EmailJS.com](https://www.emailjs.com/)
2. Connect your email service (Gmail, Outlook, etc.)
3. Create an email template (see below)
4. Get your credentials:
   - **Public Key**: Account > General > Public Key
   - **Service ID**: Email Services > Your Service ID
   - **Template ID**: Email Templates > Your Template ID

#### Step 3: Update config.js

Open `config.js` and add your credentials:

```javascript
const EMAILJS_CONFIG = {
    PUBLIC_KEY: 'your_actual_public_key',
    SERVICE_ID: 'your_actual_service_id',
    TEMPLATE_ID: 'your_actual_template_id'
};
```

### 2. Email Template

Use this HTML template in your EmailJS dashboard:

**Subject:** `🚀 New Clever Cloud Morocco Application - {{full_name}}`

**Content:** See the full HTML template in the setup guide.

### 3. Git Safety

- `config.js` is in `.gitignore` and will NOT be pushed to Git
- Only `config.example.js` is tracked in version control
- Never commit your actual API keys!

### 4. Testing

1. Open `index.html` in your browser
2. Fill out the application form
3. Submit and check your email inbox
4. You should receive a beautifully formatted email with all the form data

## 📝 Form Fields

The contact form captures:
- Full Name
- Professional Email
- Phone Number
- Organization Name
- Job Title
- Organization Size
- Use Case Description

## 🔒 Security

- API keys are stored in `config.js` (not tracked by Git)
- Client-side validation prevents empty submissions
- EmailJS handles rate limiting (200 emails/month on free tier)

## 🎨 Features

- ✅ Smooth scrolling navigation
- ✅ Responsive design
- ✅ Form validation
- ✅ Loading states
- ✅ Success/error messages
- ✅ Professional email templates
- ✅ Mobile-friendly
- ✅ FAQ accordion
- ✅ Multiple SVG icons

## 📧 Support

For questions or issues, contact: contact@clevercloud.ma
