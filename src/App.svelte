<script>
  import { onMount } from 'svelte';
</script>

<main >
  <table class="styled-table">
    <thead>
      <tr>
        <th>Year</th>
        <th>CSS Specification</th>
        <th>Color</th>
        <th>Flexbox</th>
        <th>Grid</th>
        <th>Animations</th>
        <th>Transitions</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>1996</td>
        <td><a href="https://www.w3.org/TR/REC-CSS1-961217" target="_blank" rel="noopener noreferrer">CSS1</a></td>
        <td><a href="https://www.w3.org/TR/REC-CSS1-961217#color-and-background-properties" target="_blank" rel="noopener noreferrer">Color in CSS1</a></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
      </tr>
      <tr>
        <td>1998</td>
        <td><a href="https://www.w3.org/TR/1998/REC-CSS2-19980512/" target="_blank" rel="noopener noreferrer">CSS2</a></td>
        <td><a href="https://www.w3.org/TR/1998/REC-CSS2-19980512/#color-units" target="_blank" rel="noopener noreferrer">Color in CSS2</a></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
      </tr>
      <tr>
        <td>2011</td>
        <td><a href="https://www.w3.org/TR/CSS2/" target="_blank" rel="noopener noreferrer">CSS2.1</a></td>
        <td><a href="https://www.w3.org/TR/CSS2/#color-units" target="_blank" rel="noopener noreferrer">Color in CSS2.1</a></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
      </tr>
      <tr>
        <td>2018</td>
        <td></td>
        <td><a href="https://www.w3.org/TR/css-color-3/" target="_blank" rel="noopener noreferrer">Color 3</a></td>
        <td><a href="https://www.w3.org/TR/css-flexbox-1/" target="_blank" rel="noopener noreferrer">Flexbox 1</a></td>
        <td></td>
        <td></td>
        <td></td>
      </tr>
      <tr>
        <td>2017</td>
        <td></td>
        <td></td>
        <td></td>
        <td><a href="https://www.w3.org/TR/css-grid-1/" target="_blank" rel="noopener noreferrer">Grid 1</a></td>
        <td></td>
        <td></td>
      </tr>
      <tr>
        <td>2020</td>
        <td></td>
        <td></td>
        <td></td>
        <td><a href="https://www.w3.org/TR/css-grid-2/" target="_blank" rel="noopener noreferrer">Grid 2</a></td>
        <td></td>
        <td></td>
      </tr>
      <tr>
        <td>2022</td>
        <td></td>
        <td><a href="https://www.w3.org/TR/css-color-4/" target="_blank" rel="noopener noreferrer">Color 4</a></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
      </tr>
      <tr>
        <td>2023</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td><a href="https://www.w3.org/TR/css-animations-1/" target="_blank" rel="noopener noreferrer">Animations 1</a></td>
        <td><a href="https://www.w3.org/TR/css-transitions-1/" target="_blank" rel="noopener noreferrer">Transitions 1</a></td>
      </tr>
      <tr>
        <td>2023</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td><a href="https://www.w3.org/TR/css-animations-2/" target="_blank" rel="noopener noreferrer">Animations 2</a></td>
        <td><a href="https://www.w3.org/TR/css-transitions-2/" target="_blank" rel="noopener noreferrer">Transitions 2</a></td>
      </tr>
    </tbody>
  </table>
</main>

<style>

  .styled-table {
    width: 100%;
    max-width: 1200px;
    background: #1e293b;
    border: 1px solid #334155;
  }

  .styled-table th {
    background: linear-gradient(135deg, #312e81 0%, #1e1b4b 100%);
    color: #e2e8f0;
    font-weight: 600;
    padding: 1.25rem;
    text-align: left;
    text-transform: uppercase;
    font-size: 0.875rem;
    letter-spacing: 0.05em;
    border-bottom: 2px solid #4f46e5;
  }

  .styled-table td {
    padding: 1.25rem;
    border-bottom: 1px solid #334155;
    font-size: 0.95rem;
    color: #e2e8f0;
  }

  .styled-table tr:last-child td {
    border-bottom: none;
  }

  .styled-table tbody tr {
    transition: all 0.3s ease;
  }

  .styled-table tbody tr:hover {
    background-color: #2d3748;
    transform: translateX(6px);
  }

  .styled-table a {
    color: #818cf8;
    text-decoration: none;
    position: relative;
    font-weight: 500;
    transition: all 0.3s ease;
    padding: 0.2em 0.4em;
    border-radius: 4px;
  }

  .styled-table a:hover {
    color: #c7d2fe;
    background: rgba(99, 102, 241, 0.1);
    box-shadow: 0 0 20px rgba(99, 102, 241, 0.2);
  }

  .styled-table td:first-child {
    font-weight: 600;
    color: #818cf8;
  }

  @media (max-width: 768px) {
    .styled-table {
      font-size: 0.875rem;
    }
    
    .styled-table th,
    .styled-table td {
      padding: 1rem;
    }
  }

  /* Empty cell styling */
  .styled-table td:empty {
    background: rgba(99, 102, 241, 0.05);
  }

  /* Subtle animation for empty cells */
  .styled-table td:empty::after {
    content: '—';
    color: #475569;
    opacity: 0.5;
  }
</style>