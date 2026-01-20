# This application was built by entering the following request into cursor chat:

09-cursor-built-UI-header-home-and-profile-pages
please build me a react router application using react router 8 using tailwind and shadcn

it should have a header containing

- search bar

- text "home" nav link

- text "profile" nav link

- account icon

- dark/light mode button which works

the home link should make the home page appear below the header

the profile link should make the profile page appear below the header

the account icon should instantiate a dropdown which either says login or logout depending on the "authenticated" value stored in react context

the dark/light state should also be held in react context

THEN

please upgrade this project to typescript

THEN

please upgrade this project to tailwind version 4 and remove the postcss processor in the process, please make sure it is compatible with tailwind's recommendations for working with vite

these recommendations can be found on this webpage
https://tailwindcss.com/docs/installation/using-vite

THEN

could you please convert the home and profile pages to use shadcn with the minimum number of lines possible

also I notice that there is no components.json file which the current version of shadcn uses ... could you please make sure this application looks like it has been installed by npx shadcn@latest and uses a components file

Everything below this line was created by Cursor

# React Router App with Tailwind & shadcn/ui

A React Router application built with React Router v6, Tailwind CSS, and shadcn/ui components.

## Features

- **React Router**: Navigation between Home and Profile pages
- **Tailwind CSS**: Utility-first CSS framework
- **shadcn/ui**: Beautiful, accessible component library
- **Dark/Light Mode**: Theme toggle with React Context
- **Authentication Context**: Login/Logout state management
- **Responsive Header**: Search bar, navigation links, account dropdown, and theme toggle

## Getting Started

### Installation

```bash
npm install
```

### Development

```bash
npm run dev
```

The app will be available at `http://localhost:5173`

### Build

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

## Project Structure

```
src/
  ├── components/
  │   ├── ui/          # shadcn/ui components
  │   └── Header.jsx   # Main header component
  ├── contexts/        # React Context providers
  │   ├── AuthContext.jsx
  │   └── ThemeContext.jsx
  ├── pages/           # Page components
  │   ├── Home.jsx
  │   └── Profile.jsx
  ├── lib/             # Utility functions
  │   └── utils.js
  ├── App.jsx          # Main app component with routing
  ├── main.jsx         # Entry point
  └── index.css        # Tailwind styles
```

## Features Breakdown

### Header Component

- **Search Bar**: Functional search input with icon
- **Navigation Links**: "Home" and "Profile" links that highlight when active
- **Account Icon**: Dropdown menu showing "Login" or "Logout" based on auth state
- **Theme Toggle**: Button to switch between dark and light mode

### Authentication

- Managed via React Context (`AuthContext`)
- Toggle authentication state by clicking Login/Logout in account dropdown
- Profile page shows authentication status

### Theme

- Managed via React Context (`ThemeContext`)
- Persists theme preference in localStorage
- Applies dark mode class to document root
