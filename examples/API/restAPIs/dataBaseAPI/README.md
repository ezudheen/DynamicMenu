# Database API

##  Functions 
### createTable 
  Arguments:   
  xml: the xml request as string
### deleteTable
  Arguments:  
  tableName : string
### modifyTable
  Arguments:  
  tableName: string  
  xml : xml request as string
### insertData
  Arguments:  
  xml: xml request as string  
### deleteData
  Arguments:  
  xml: xml request as string
### updateData
  Arguments:  
  xml: xml request as string
### showData
  Arguments:
  xml: xml request as string
  
  
## XML format
* Arguments  
```
<db_op_arg>
	<db_name>
		name of the db
	</db_name>	
	<db_operation>
		create_table/inert_data/...
	</db_operation>	
	<table_name>
		name of the table
	</table_name>
	<table_header>
		<column1>
			<name_field>
				name of field1
			</name_field>
			<data_type_field>
				data_type of field1
			</data_type_field>
		</column1>
		<column2>
			<name_field>
				name of field2
			</name_field>
			<data_type_field>
				data_type of field2
			</data_type_field>
		</column2>
	</table_header>
	<table_row>
		<column1>
			<value_field>
				value of field1
			</value_field>
		</column1>
		<column2>
			<value_field>
				value of field2
			</value_field>
		</column2>
	</table_row>
</db_op_arg>
```
* Return value  
```
<db_op_ret>
	<db_name>
		name of the db
	</db_name>	
	<db_operation>
		create_table/inert_data/...
	</db_operation>
	<db_operation_status>
		successful/failed
	</db_operation_status>		
	<table_name>
		name of the table
	</table_name>
	<table_header>
		<column1>
			<name_field>
				name of field1
			</name_field>
			<data_type_field>
				data_type of field1
			</data_type_field>
		</column1>
		<column2>
			<name_field>
				name of field2
			</name_field>
			<data_type_field>
				data_type of field2
			</data_type_field>
		</column2>
	</table_header>
	<table_row>
		<column1>
			<value_field>
				value of field1
			</value_field>
		</column1>
		<column2>
			<value_field>
				value of field2
			</value_field>
		</column2>
	</table_row>
</db_op_ret>
```
