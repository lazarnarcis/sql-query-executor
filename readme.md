# sql-query-executor

## Examples: (functions: insert, query, update, where, select, deleteRow, deleteColumn, addColumn)

### insert() function
$data = array("column", "value");
$database->insert("table_name", $data);

### query() function
$query = "SELECT * FROM table_name";
$database->query($query);

### where() function
$database->where("column", "value"); // where condition

### update() function
$data = array("column", "value");
$database->where("column", "value"); // where condition
$database->update("table_name", $data);

### select() function
$database->select("table_name", /*LIMIT (not required)*/);

### deleteColumn() function
$database->deleteColumn("table_name", "column_name");

### deleteRow() function
$database->where("column", "value"); // where condition
$database->deleteRow("table_name");

### addColumn() function
$database->addColumn("table_name", "column_name", "column_type", "column_value");