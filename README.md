# ConceptARC Visualizer

A web-based interactive visualizer for exploring ConceptARC data and human abstraction patterns. This tool provides an intuitive interface for analyzing AI model performance, rule identification, and validation across different concepts and test cases.

## Features

- **Interactive Grid Visualization**: Faithful color representation with dynamic scaling
- **Rule Analysis**: Compare model-identified rules with ground truth and human descriptions
- **Validation Tools**: Built-in system for marking rule correctness and importance
- **Performance Tracking**: Real-time indicators showing concept-level accuracy
- **Human Mode**: Specialized interface for analyzing human-generated rules
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices

## Usage

1. **Load Data**: Click "Load CSV" to upload your ConceptARC evaluation data
2. **Navigate**: Use dropdown menus to select puzzles, tests, and concepts
3. **Explore**: View training demonstrations, test inputs, and model outputs
4. **Validate**: Use validation tools to mark rule correctness and importance
5. **Compare**: Switch between standard and human modes for different data types

## File Structure

- `index.html` - Main page with embedded visualizer
- `visualizer.js` - Core visualizer functionality
- `visualizer.css` - Styling and responsive design
- `README.md` - This documentation

## Data Format

The visualizer expects CSV files with the following columns:

### Standard Mode
- `puzzle` - Puzzle identifier
- `test_idx` - Test index
- `answer` - Model's answer (grid format)
- `Rule` - Model-identified rule
- `summary` - Model reasoning summary
- `is_correct` - Binary correctness indicator

### Human Mode
- `Task` - Task/puzzle path
- `Test` - Test number
- `VerbalDescription` - Human rule description
- `Rule_correct_label` - Validation label
- `validation_level` - Validation level
- `starred` - Starred status

## Technical Details

- **Grid Rendering**: Canvas-based rendering with faithful ARC color palette
- **Responsive Design**: CSS Grid and Flexbox for optimal layout
- **Dark Mode**: Automatic dark mode detection and styling
- **Performance**: Optimized for large datasets with efficient rendering

## Browser Support

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+
