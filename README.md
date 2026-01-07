# 🚀 TaskGlitch - Sales Task Management

A high-performance Task Management Web App designed for sales teams to track, prioritize, and analyze tasks based on ROI. This project was part of a bug-fixing challenge to ensure stability, deterministic logic, and a premium user experience.

👉 **[Live Demo](https://erino-assignment-48u7hr0on-aryapkar-7543s-projects.vercel.app)**

---

## 🛠️ Tech Stack

- **Framework**: React 18
- **Styling**: Material UI (MUI)
- **State Management**: React Context API + Custom Hooks
- **Persistence**: LocalStorage
- **Build Tool**: Vite + TypeScript

---

## ✨ Features

- **ROI-Driven Prioritization**: Automatically calculates ROI (Revenue ÷ Time) to help you focus on high-impact tasks.
- **Dynamic Insights**: Real-time metrics including Total Revenue, Efficiency, and Average ROI.
- **Advanced Sorting**: Nested sorting by ROI, Priority (High/Medium/Low), and deterministic tie-breakers.
- **Undo Functionality**: Accidental deletion protection with a timed snackbar-based undo.
- **CSV Support**: Bulk import and export functionality for easy data management.
- **Responsive Design**: Polished, mobile-friendly interface with consistent typography and spacing.

---

## 🐞 Bug Fixes Implemented

Each bug was addressed with detailed attention to performance and standard coding practices:

| Bug ID | Title | Description | Fix Implemented |
| :--- | :--- | :--- | :--- |
| **BUG 1** | **Double Fetch** | API/Data fetch was called twice on startup. | Removed redundant effects and optimized initial load strategy. |
| **BUG 2** | **Undo State Leak** | Deleted state wasn't clearing after snackbar closed. | Implemented proper state cleanup when the undo window closes. |
| **BUG 3** | **Unstable Sorting** | ROI ties caused flickering and random reordering. | Introduced a deterministic alphabetical tie-breaker. |
| **BUG 4** | **Double Dialog** | Clicking Edit/Delete triggered multiple dialogs. | Implemented `stopPropagation` to manage event bubbling correctly. |
| **BUG 5** | **ROI Validation** | Division by zero and NaN values in calculations. | Added robust validation for 0-time inputs and 2-decimal formatting. |

---

## 💻 Installation & Local Setup

To run this project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/AryaP-1243/erino-assignment.git
   cd erino-assignment
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Start the development server**:
   ```bash
   npm run dev
   ```

4. **Build for production**:
   ```bash
   npm run build
   ```

---

## 🚢 Deployment

The project is configured for seamless deployment on **Vercel**.

To deploy your own version:
```bash
vercel --prod
```

---

## 📄 License

This project is part of a coding assignment and is provided as-is for evaluation purposes.
