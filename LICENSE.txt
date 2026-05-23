@tailwind base;
@tailwind components;
@tailwind utilities;

.tab-btn {
  padding: 12px 20px;
  font-weight: 500;
  color: #4b5563;
  transition: all 0.2s;
}

.tab-btn.active {
  color: #1e40af;
  border-bottom: 4px solid #1e40af;
  font-weight: 600;
}

table td, table th {
  padding: 12px 16px;
  border-bottom: 1px solid #e5e7eb;
}

tr:hover {
  background-color: #f8fafc;
}