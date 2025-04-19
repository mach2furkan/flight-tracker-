# flight-tracker-



# ✈️ Flight Tracking System

A sleek, real-time **Flight Tracker Dashboard** built using simulated flight data, custom SVG map rendering, and a powerful modern UI. Designed as an alternative to services like FlightRadar24 — no public API? No problem.

> ⚠️ **Note:** This is a simulation. No actual flight APIs are used — just beautifully realistic generated data.

---

## 🌐 Live Demo
[🚀 Deploy your own version](#) (Coming soon…)

---

## 🧩 Features

- 🗺️ **Interactive Map Display**  
  Custom-built SVG world map that shows all flights with airplane icons, rotating to match heading.

- 🔄 **Real-Time Simulated Updates**  
  Flight positions update every 5 seconds for a real-time experience.

- 🔍 **Flight Search & Filtering**  
  Search by flight number, airline, or route. Filter by altitude, airline, and more.

- 📊 **Detailed Flight Info**  
  Altitude, speed, heading, origin/destination, aircraft type, and more — just a click away.

- 🌦️ **Weather Simulation**  
  Simulated weather data for origin, destination, and en-route visibility.

- 📈 **Flight Timeline**  
  Progress tracker from departure to arrival.

- 📱 **Fully Responsive Design**  
  Clean layout with `shadcn/ui` that adapts beautifully to all screen sizes.

---

## 🔧 How It Works

The system simulates real-world flights between major global airports. Each flight:

- Has a unique flight number, airline, registration, and route
- Moves along a generated flight path
- Updates position and metadata periodically
- Can be interacted with on the map or via the sidebar list

> Originally built with `react-map-gl`, now updated to use a custom SVG-based map to avoid MIME-type errors in preview environments.

---

## 🛠️ Tech Stack

| Stack         | Description |
|--------------|-------------|
| **Next.js**  | App framework for fast, modern UIs |
| **TypeScript** | Strongly typed development |
| **Mapbox** *(originally)* | Replaced with SVG custom world map |
| **shadcn/ui** | Elegant and responsive UI components |
| **Lucide Icons** | Minimal, customizable icon set |
| **Custom Data Simulator** | Generates realistic flight data dynamically |

---

## 🧪 Current Limitations

- No live data (simulated only)
- Weather is static (could be enhanced with an actual weather API)
- SVG map is simplified for performance and compatibility

---

## 💡 Future Improvements

- Integration with real flight or weather APIs
- Full-screen map mode
- Historical flight playback
- Airport info pages

---

## 🗂️ Repository Structure

```bash
📦 flight-tracker
├── components/
│   └── world-map.tsx        # SVG-based world map with interactive features
├── lib/
│   └── flight-data.ts       # Flight simulation logic
├── app/
│   └── page.tsx             # Main dashboard
├── public/
│   └── assets/              # Icons, map backgrounds, etc.
├── styles/
│   └── globals.css
```

---

## 🚧 Fixes & Notes

> 🛠️ MIME-Type Error Fix  
Replaced `react-map-gl` with a fully interactive SVG-based `WorldMap` component to avoid:
```
Failed to load "react-map-gl" from "blob:...". Modules must be served with a valid MIME type like application/javascript.
```

---

## 🔗 Repo

📁 [GitHub Repository](https://github.com/mach2furkan/flight-tracker-/upload/main)

---

## 🙌 Contributions

Open to improvements, ideas, and pull requests! Let's build this sky-high. ✈️

---

