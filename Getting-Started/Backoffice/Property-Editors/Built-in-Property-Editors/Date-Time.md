# DateTime

`Returns: DateTime`

Displays a calendar UI for selecting dates and time which is saved as a DateTime value.

## Data Type Definition Example

![Data Type Definition Example](images/Date-Time-With-Time-Data-Type.png)

The only setting which is presented in the DateTime DataType, is to alter the format of this property.
Default you have a format like `YYYY-MM-DD HH:mm:ss`, but you can easily change this to something else ( see [MomentJS.com](http://momentjs.com/) for more examples ).

## Content Example 

![Content Example](images/Date-Time-With-Time-Content.png)

## MVC View Example - displays a datetime with time 

### Typed:

	@(Model.Content.GetPropertyValue<DateTime>("datePicker").ToString("dd MM yyyy HH:mm:ss"))

### Dynamic: 

	@{
		@CurrentPage.datePicker.ToString("dd-MM-yyyy HH:mm:ss")
	}
