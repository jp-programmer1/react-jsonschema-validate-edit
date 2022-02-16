
#  react-jsonschema-validate-edit
Easy to use json schema validation editor.

##  Usage

`npm install react-jsonschema-validate-edit`

  

    import  React, { useState } from 'react';
    import { JsonSchemaValidateEdit } from 'react-jsonschema-validate-edit';
    
    const Component = () => {
	    const [jsonSchema, setJsonSchema] = useState({});
	    
	    return (
		    <JsonSchemaValidateEdit value={values} onChange={setJsonSchema} />
	    );
	  }

## Properties
| name | type | default | description |
|--|----------|------------|-------------|
| data | JsonSchema | undefined | the json schema object |
| onChange | Function Callback | null | function that returns a jsonschema |
| className | string | null |  container className |
| id | string | null  | set container id |
| componentOnCollapse | JSX | undefined | integrate component when collapsed is true |
| componentOffCollapse | JSX | undefined | integrate component when collapsed is false |
| componentRemove | JSX | undefined | integrate remove item component|
| componentAdd | JSX | undefined | integrate add item component |
| getList | array | undefined | function that returns a properties list in array object |
| showList | boolean | true | show list when adding items |
| removeItem | string | undefined | receives the name of the value you want to remove |
| onFinishedRemoveItem | Function Callback | undefined | function that warns that I delete an element |