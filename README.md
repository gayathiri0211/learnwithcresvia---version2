# 🎓 LearnWithCresvia

A modern college learning and coding platform built with React, Vite, and Supabase.

## ✨ Features

- 🔐 **Complete Authentication System**
  - Email/Password signup and login
  - Email verification
  - Session persistence
  - Password strength indicator
  - Form validation

- 🎨 **Beautiful UI/UX**
  - Modern gradient design
  - Responsive layout (mobile-first)
  - Smooth animations
  - Professional styling

- 👥 **Role-Based Access Control**
  - STUDENT
  - STAFF
  - COORDINATOR
  - HOD
  - ADMIN

- 📊 **User Profiles**
  - XP tracking
  - Streak system
  - Department assignment
  - Year tracking


   ```



## 📁 Project Structure

```
learnwithcresvia/
├── src/
│   ├── components/       # Reusable components
│   │   └── Loading.jsx
│   ├── contexts/         # React contexts
│   │   └── AuthContext.jsx
│   ├── hooks/            # Custom hooks
│   │   └── useAuth.js
│   ├── pages/            # Page components
│   │   ├── HomePage.jsx
│   │   ├── LoginPage.jsx
│   │   ├── SignupPage.jsx
│   │   ├── TestAuthPage.jsx
│   │   └── NotFound.jsx
│   ├── styles/           # CSS files
│   │   ├── index.css
│   │   └── auth.css
│   ├── utils/            # Utility functions
│   │   └── supabaseClient.js
│   ├── App.jsx           # Main app component
│   └── main.jsx          # Entry point
├── .env                  # Environment variables
├── .env.example          # Environment template
├── index.html            # HTML template
├── package.json          # Dependencies
├── vite.config.js        # Vite configuration
└── README.md             # This file
```

## 🧪 Testing

### Test Authentication

1. **Sign Up**
   - Go to `/signup`
   - Create account with email/password
   - Check email for confirmation (if enabled)
   - Verify profile created in Supabase

2. **Sign In**
   - Go to `/login`
   - Enter credentials
   - Should redirect to homepage
   - Session persists on refresh

3. **Sign Out**
   - Click sign out button
   - Should clear session
   - Redirect to login

### Test Routes

- `/` - Homepage
- `/login` - Login page
- `/signup` - Signup page
- `/test-auth` - Testing page (remove in production)


### Adding New Features

1. Create component in appropriate directory
2. Update routes in `App.jsx`
3. Add styles in `styles/` directory
4. Test functionality

## 📝 Next Steps

- [ ] Add password reset functionality
- [ ] Create role-specific dashboards
- [ ] Add course management
- [ ] Implement code editor
- [ ] Add Judge0 integration
- [ ] Build student progress tracking
- [ ] Create admin panel

## 🐛 Troubleshooting

### Common Issues

**Loading screen stuck:**
- Check browser console for errors
- Verify Supabase credentials in `.env`
- Clear browser cache and local storage

**Sign up not working:**
- Check Supabase database trigger
- Verify RLS policies
- Check browser console for errors

**Session not persisting:**
- Verify supabaseClient.js configuration
- Check browser local storage
- Ensure `persistSession: true`

## 📄 License

This project is for educational purposes.

## 👥 Contributors

- Gayathiri Goopalakrishnan - Initial work

##  Acknowledgments

- Supabase for backend infrastructure
- React team for the framework
- Vite for blazing-fast builds
