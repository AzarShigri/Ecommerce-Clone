Food Delivery App UI – React Native
Overview

This project is a modern Food Delivery Mobile App UI built using React Native.
It features a clean and attractive interface where users can browse food categories, search for meals, and view popular food items.

The project is ideal for beginners who want to learn:

React Native UI design
State management with React Hooks
Building modern mobile layouts
Working with lists and filtering
Using images in React Native
Features
Modern food delivery UI
Search bar for food items
Food category filtering
Scrollable categories section
Popular food cards with images
Ratings, prices, and delivery time display
Bottom navigation bar
Responsive mobile design
Clean and colorful interface
Technologies Used
React Native
JavaScript
React Hooks (useState)
React Native Components
Project Structure
project-folder/
│
├── App.js
├── package.json
└── README.md
Installation
1. Create React Native Project

Using Expo:

npx create-expo-app food-delivery-ui
2. Move to Project Folder
cd food-delivery-ui
3. Replace App.js

Replace the default App.js file with the provided code.

4. Install Dependencies
npm install
5. Run the Project
npx expo start
App Screens
Home Screen UI
4
How It Works
Search Functionality

The app stores search text using:

const [search, setSearch] = useState('');

Users can type food names in the search bar.

Category Filtering

Food categories are filtered using:

const filteredFoods = selectedCategory === 'All'
  ? foods
  : foods.filter(f => f.name.includes(selectedCategory));

When a category is selected, only matching food items are displayed.

Food Data

Food items are stored inside an array:

const foods = [
  {
    id: 1,
    name: 'Margherita Pizza',
    price: '$12.99'
  }
]

Each item contains:

Name
Price
Rating
Delivery time
Food image
Components Used
Component	Purpose
View	Layout container
Text	Display text
ScrollView	Scrollable content
TextInput	Search field
TouchableOpacity	Buttons
Image	Food images
SafeAreaView	Safe mobile screen layout
StatusBar	Status bar customization
UI Sections
Header

Displays:

Greeting text
User location
Profile button
Search Bar

Allows users to search for food items.

Promotional Banner

Shows discount offers for users.

Categories Section

Users can select:

Pizza
Burger
Drinks
Desserts
Food Cards

Each card contains:

Food image
Food name
Price
Rating
Delivery time
Bottom Navigation

Navigation tabs:

Home
Search
Cart
Profile
Future Improvements

You can enhance this project by adding:

Real backend integration
Firebase authentication
Cart functionality
Payment gateway
Favorite items
Order tracking
Real-time delivery status
API integration
Dark mode support
Learning Outcomes

After completing this project, you will understand:

React Native fundamentals
Mobile UI/UX design
State management
Dynamic rendering
Array filtering
Responsive layouts
Component styling
Author

Created by M. Raza

License

This project is open-source and free for educational purposes.
