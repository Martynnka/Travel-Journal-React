# Travel Journal – React Project

This project is a small **React application** that displays travel journal entries.  
It was built as part of the **Scrimba React course** to practice core React concepts such as components, props, and dynamic rendering.

The application shows a list of travel locations with images, descriptions, dates, and links to Google Maps.

---

## 🚀 Features

- Built with **React + Vite**
- Reusable **React components**
- Data-driven rendering using **JavaScript arrays**
- Use of **props** to pass data to components
- Dynamic rendering with **.map()**
- Clean component structure

---

## 🧠 What I Practiced

This project helped me understand:

- React component structure
- Passing data using **props**
- Using the **spread operator (`...props`)**
- Rendering lists in React with `.map()`
- Organizing projects into **components and data files**

---

## 🧩 Project Structure


├── components
│ ├── Header.jsx
│ └── Entry.jsx
├── images
│ ├── globe.png
│ └── marker.png
├── data.js
├── App.jsx
├── index.jsx
├── index.css
└── index.html


**Main components**

- `Header.jsx` – Displays the application header
- `Entry.jsx` – Displays individual travel journal entries
- `data.js` – Contains the travel data used to render entries

---

## ⚙️ How It Works

The application imports travel data from `data.js` and dynamically renders each entry.

Example logic:

```javascript
const entryElements = data.map((entry) => {
    return (
        <Entry
            key={entry.id}
            {...entry}
        />
    )
})
