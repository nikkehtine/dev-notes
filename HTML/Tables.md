# Tables

## Basic structure

```html
<table>
	<tr>
		<th>Name</th>
		<th>Age</th>
		 
	</tr>
	<tr>
		<td>Amy</td>
		<td>42</td>
	</tr>
	<tr>
		<td>Bob</td>
		<td>19</td>
	</tr>
</table>
```

- `<table>` is the main table element
- `<tr>` is the table row of cells
- `<td>` is the table cell (data cell)
- `<th>` is the table header cell

## Table with sections and spanning

```html
<table>
	<thead>
		<tr>
			<th colspan="2">The table header</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>The table body</td>
			<td>with two columns</td>
		</tr>
	</tbody>
</table>
```

- `<thead>` defines a set of rows defining the head of the table
- `<tbody>` encapsulates a set of table rows that make up the body of the table

- `colspan` allows a column to span multiple cells
- `rowspan` allows a cell to span multiple rows
