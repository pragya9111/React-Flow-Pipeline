# React Pipeline Builder

This project is a visual pipeline builder with a React-based frontend and a FastAPI backend. Users can drag and drop nodes, connect them, and analyze pipeline structure.

## Folder Structure

```
backend/
  main.py                # FastAPI backend for pipeline analysis
frontend/
  package.json           # React app dependencies and scripts
  public/                # Static assets and HTML template
  src/                   # React source code
    App.js
    store.js
    ui.js
    toolbar.js
    submit.js
    draggableNode.js
    components/
      BaseNode.js
      NodeStyles.js
    nodes/
      inputNode.js
      llmNode.js
      outputNode.js
      textNode.js
      customNodes/
        ToggleNode.js
```

## Features

- **Drag-and-drop interface:** Easily add, move, and connect nodes to build custom pipelines.
- **Custom node types:** Includes input, output, text, LLM, and toggle nodes. Extendable for more node types.
- **Real-time validation:** Backend analyzes pipeline structure and provides feedback.
- **Separation of concerns:** Cleanly separated frontend (React) and backend (FastAPI) for scalability and maintainability.

## Basic Commands

### Frontend

- **Install dependencies:**  
  `npm install`

- **Start development server:**  
  `npm start`

- **Build for production:**  
  `npm run build`

### Backend

- **Install dependencies:**  
  `pip install fastapi uvicorn networkx`

- **Run backend server:**  
  `uvicorn main:app --reload --host 0.0.0.0 --port 8000`

---

For more details, see the comments in each file.
