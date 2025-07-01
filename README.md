
# 📱 CitizenConnect – Complaint Raising Application

A full-featured, mobile-first complaint tracking and resolution system built with **React Native**. Citizens can easily submit complaints, attach evidence (images), choose relevant departments, receive real-time status updates, and interact with authorities via a notification-driven system. Also includes story-based updates and user profile management.

---

## 🚀 Features

### 📝 Complaint Management
- Raise complaints with title, description, and images
- Select department (e.g., Water, Roads, Electricity, etc.)
- Choose between **current location** or **searched address**
- Track complaint lifecycle through **visual timelines**
- Mark complaints as **Completed**

### 🔔 Notifications
- Receive and view complaint-specific updates in real time
- Dynamic rendering with rich HTML content and status labels

### 📸 Stories (24H)
- Post stories with captions and images
- Swipe left/right/down to browse and exit
- Delete story if posted by current user

### 👤 User Profile
- Sign up, log in, and reset password via Firebase
- Update profile (name, phone, bio, username, and image)
- Account deletion confirmation via WebView

### 🌍 Location & Maps
- Uses **Expo Location** API to fetch current address
- Integrates **Google Places API** for location search and autocomplete

---

## 🧑‍💻 Tech Stack

| Layer | Technologies |
|-------|--------------|
| **Frontend** | React Native, Expo Router, React Navigation |
| **Backend** | Firebase (Auth, Firestore, Storage) |
| **State Management** | React Context API |
| **Location & Maps** | Expo Location API, Google Places API |
| **Styling** | Responsive Design (`react-native-responsive-screen`), Custom Font (`Poppins`) |
| **Animations & SVG** | Lottie, SVG XMLs |
| **Others** | Day.js, Gesture Recognizer, Alert API, FlatList, Pressable |

---

## 📁 Project Structure

```bash
.
├── app/
│   ├── (tabs)/         # Home, Add, Edit (Complaints), Profile Tabs
│   ├── (auth)/         # Login, Signup, Forgot Password
│   ├── (app)/          # Post view, Notification, Story viewer, Profile update
│   └── index.js        # Entry point
├── components/         # Reusable UI components
├── constants/          # Colors, APIs, Departments, States
├── context/            # Auth context and global state
├── firebase/           # Firebase initialization (auth, db, storage)
├── assets/             # SVGs, fonts, animations, app logo
├── app.json / eas.json / babel.config.js
└── package.json
```

---

## 🛠️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/citizenconnect-app.git
cd citizenconnect-app
```

### 2. Install Dependencies

```bash
npm install
# or
yarn install
```

### 3. Setup Firebase

- Create a Firebase project.
- Enable Email/Password Authentication.
- Set up Firestore Database and Storage.
- Replace your Firebase config in `firebase/index.js`.

### 4. Add Google Maps API Key

- Enable **Geocoding API** and **Places API** in Google Cloud.
- Replace API key inside:
  - `edit.js` → for Geolocation & Places Autocomplete
  - **(Move it to `.env` in production!)**

### 5. Run the App

```bash
npx expo start
```

---

## ⚠️ Environment Variables (Recommended)

Create a `.env` file:

```
GOOGLE_MAPS_API_KEY=your_google_api_key
FIREBASE_API_KEY=your_firebase_key
...
```

Then use a `.env` loader (like `babel-plugin-dotenv` or `expo-constants`) for secure access.


## ✨ Contributions

PRs are welcome! Please:
- Fork the repo
- Create a new branch (`feature/xyz`)
- Open a pull request with a clear description

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 🙌 Acknowledgements

- [Firebase](https://firebase.google.com/)
- [Google Maps Platform](https://developers.google.com/maps)
- [React Native](https://reactnative.dev/)
- [Expo](https://expo.dev/)
- Icons from [Icons8](https://icons8.com)

---

## 👨‍💻 Author

**Sai Cheboina**  
Senior Software Engineer | DevOps + Fullstack  
🔗 [LinkedIn](https://linkedin.com/in/saicheboina)  
📧 saicheboina@email.com
