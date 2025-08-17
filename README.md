# NeuroLearn - AI-Powered Education App

A comprehensive learning platform with personalized authentication and grade-based subject selection.

## Features

### Authentication System
- **Sign Up**: Complete registration with grade-based subject selection
- **Sign In**: Secure login with email and password
- **User Profile**: Stores user preferences and academic information

### Grade-Based Subject Selection

#### Grades 1-5
- **Subjects**: Tamil, Maths, Religion, English, Sinhala, Social Science (Sutradal)
- **Medium**: Tamil or English

#### Grades 6-9
- **Subjects**: Tamil, Religion, Maths, History, Science, Civics, Geography, English, ICT, Art, Dance, Music, Sinhala
- **Medium**: Tamil or English

#### Grades 10-11
- **Core Subjects**: Tamil, Maths, Science, History, English, Religion
- **Basket Subjects** (Select 3):
  - **Basket 1**: Civics, Geography, Business, Accounting Studies
  - **Basket 2**: Art, Music, Dance, Sinhala Literature, Tamil Literature, English Literature
  - **Basket 3**: ICT, Health Science, Agriculture, Home Economics
- **Medium**: Tamil or English

#### Grades 12-13 (A/L)
- **Core Subjects**: Tamil, Maths, Science, History, English, Religion
- **Streams**:
  - **Arts Stream**: Social Sciences, Languages, Aesthetic Subjects, Religious Studies, Technological Subjects
  - **Science Stream**: Mathematics, Physics, Chemistry, Biology, ICT, Agriculture
  - **Commerce Stream**: Economics, Accounting, Business Studies, ICT
  - **Technology Stream**: Science for Technology, Engineering Technology, Bio Systems Technology, ICT, Agriculture, Geography, Higher Mathematics, Home Economics
- **Medium**: Tamil or English

### Personalized Learning Experience
- Lessons are filtered based on user's grade and selected subjects
- Language interface adapts to user's medium preference (Tamil/English)
- Progress tracking for each subject
- AI-powered tutoring system

## Getting Started

1. **Install Dependencies**
   ```bash
   npm install
   ```

2. **Start Development Server**
   ```bash
   npm run dev
   ```

3. **Access the Application**
   - Open your browser and navigate to `http://localhost:5173`
   - You'll be redirected to the authentication page
   - Create a new account or sign in with existing credentials

## Usage

### Creating an Account
1. Click "Sign Up" on the authentication page
2. Fill in your details:
   - Student Name
   - Grade (1-13)
   - Select basket subjects (for grades 10-11)
   - Choose stream (for grades 12-13)
   - Select medium (Tamil or English)
   - Email and password
3. Click "Create Account"

### Signing In
1. Enter your email and password
2. Click "Sign In"
3. You'll be redirected to your personalized dashboard

### Navigating the App
- **Dashboard**: Overview of your learning progress
- **Lessons**: Access lessons based on your grade and subjects
- **AI Tutor**: Get personalized help and explanations
- **Progress**: Track your learning achievements
- **Profile**: View and edit your account information

## Technical Stack

- **Frontend**: React with TypeScript
- **UI Components**: Radix UI with custom styling
- **Styling**: Tailwind CSS
- **State Management**: React Context API
- **Routing**: React Router
- **Build Tool**: Vite

## Project Structure

```
src/
├── components/
│   ├── auth/           # Authentication components
│   ├── ui/            # Reusable UI components
│   └── ...            # Feature components
├── contexts/          # React contexts
├── data/              # Static data and configurations
├── pages/             # Page components
└── ...
```

## Authentication Flow

1. **Unauthenticated State**: Users see the authentication page
2. **Sign Up Process**: 
   - Grade selection determines available subjects
   - Basket subjects for grades 10-11
   - Stream selection for grades 12-13
   - Medium preference stored
3. **Sign In Process**: Validates credentials and loads user data
4. **Authenticated State**: Access to personalized learning content

## Customization

### Adding New Subjects
Edit `src/data/subjects.ts` to add new subjects for specific grades.

### Modifying Lesson Content
Update the lesson templates in `src/components/LessonsPage.tsx` to customize lesson content.

### Language Support
Add new translations to the translation objects in each component.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is licensed under the MIT License. 