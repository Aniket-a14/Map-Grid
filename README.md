# Map Application Upgrade

This project is a React-based single-page application for creating and managing Areas of Interest (AOIs) on a map. It features satellite imagery from NRW WMS, polygon drawing capabilities, and a modern UI.

## 📚 Documentation

For detailed setup instructions, architecture decisions, and API documentation, please refer to [documentation.md](./documentation.md).

## 🛠 Tech Stack

- **Frontend**: React, TypeScript, Vite
- **Styling**: Tailwind CSS
- **Map Engine**: MapLibre GL JS
- **State Management**: Zustand
- **Testing**: Vitest (Unit), Playwright (E2E)
- **Geocoding**: Nominatim API (via Axios)

## ✅ Success Criteria Met
1.  **Clean, Maintainable Code**:
    -   Strict separation of concerns: Map logic (`MapView`), UI (`Sidebar`), and State (`useAOIStore`).
    -   Type-safe codebase with TypeScript.
    -   Enforced code style with **Prettier** and **ESLint**.
2.  **Thoughtful Component Structure**:
    -   Modular components (`DrawingTools`, `SearchBar`) that are easily testable and reusable.
    -   Zustand store acts as the single source of truth, preventing prop drilling.
3.  **Appropriate Test Coverage**:
    -   **E2E**: Playwright tests cover critical user flows (Map load, Layer toggle).
    -   **Unit**: Vitest tests cover UI logic (`Sidebar`).
4.  **Performance-Conscious**:
    -   **WebGL**: MapLibre handles large datasets efficiently.
    -   **Optimized State**: Zustand avoids unnecessary re-renders.
5.  **Bonus Features**:
    -   **Full-Screen Toggle**: Implemented.
    -   **Accessibility**: ARIA labels and keyboard navigation support.
    -   **Persistence**: AOIs saved to `localStorage`.
    -   **Search**: Integrated Nominatim geocoding.

## 📄 License

This project is licensed under the MIT License.
