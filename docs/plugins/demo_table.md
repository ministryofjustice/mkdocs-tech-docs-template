---
hide:
  - toc
---

# Example Table

Uses the following plugins and customisation:

- [mkdocs-table-reader-plugin](https://timvink.github.io/mkdocs-table-reader-plugin/) to convert [`example_table.csv`](./example_table.csv) into a markdown table.
- [tablesort](http://tristen.ca/tablesort/demo/) to make the table sortable
- Custom javascript to filter by the first column in the table

<input type="text" id="myInput" onkeyup="myFunction()" placeholder="Search for ..." title="Type in a name">

{{ read_csv('docs/plugins/demo_table.csv') }}

<script src="https://unpkg.com/tablesort@5.3.0/dist/tablesort.min.js"></script>
<script>
  var tables = document.querySelectorAll("article table:not([class])")
  tables.forEach(function(table) {
    new Tablesort(table)
  })
</script>
<script>
  function myFunction() {
    var input, filter, tables, table, tr, td, i;
    input = document.getElementById("myInput");
    filter = input.value.toUpperCase();
    tables = document.querySelectorAll("article table:not([class])")
    table = tables.item(tables.length - 1)
    tr = table.getElementsByTagName("tr");
    for (i = 0; i < tr.length; i++) {
      td = tr[i].getElementsByTagName("td")[0];
      if (td) {
        if (td.innerHTML.toUpperCase().indexOf(filter) > -1) {
          tr[i].style.display = "";
        } else {
          tr[i].style.display = "none";
        }
      }       
    }
  }
</script>