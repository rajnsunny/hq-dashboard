# HireQuotient Assignment
[YOUTUBE](https://youtu.be/WuaqC5iX458)     
[LIVE LINK](https://hq-dashboard.netlify.app/)
```markdown
# DataTable Component

The DataTable component is a React component that leverages the Material-UI DataGrid to display and manage tabular data with features such as search, pagination, row actions, and more.

## Features

- Search functionality for filtering data based on user input.
- Bulk deletion of selected rows.
- Edit, Save, Cancel, and Delete actions for individual rows.
- Pagination for navigating through the data.
- Responsive design with the Material-UI DataGrid.

## Installation

To use the DataTable component in your React application, follow these steps:

1. Install Material-UI DataGrid and other required dependencies:

```bash
npm install @mui/x-data-grid @mui/material
```

2. Include the DataTable component in your project:

```bash
# Assuming your DataTable component is in the components folder
# Replace path accordingly if your structure is different
cp path/to/DataTable.jsx src/components/
```

## Usage

Import the DataTable component and use it in your application. Here's an example:

```jsx
import DataTable from './components/DataTable/DataTable';
import { columns } from './utility/tabledata';

const YourApp = () => {
  // Your data source
  const data = [
    // ... your data
  ];

  // Your delete handlers
  const handleDeleteMultiple = (selectedRows) => {
    // ... your logic for deleting multiple rows
  };

  const handleDeleteSingle = (rowId) => {
    // ... your logic for deleting a single row
  };

  return (
    <div>
      <DataTable
        originalData={data}
        handleDeleteMultiple={handleDeleteMultiple}
        handleDeleteSingle={handleDeleteSingle}
      />
    </div>
  );
};
```

## Props

- **originalData**: An array of objects representing the initial data.
- **handleDeleteMultiple**: A function to handle the deletion of multiple selected rows.
- **handleDeleteSingle**: A function to handle the deletion of a single row.



