# Deep Dive: Advanced workflow automation with Microsoft Flow (Stephen Siciliano)

Part of Business Application Platform

Flow + PowerApps go hand-in-hand to create automated processes.

## Triggers and Actions

Triggers at the beginning of flow, then tasks run throughout the Flow.

3 ways to 
Run manually
Run on a schedule
Run on an event (on-prem or cloud)

Actions - steps that actually run after the trigger.

Actions that don't connect to anything are called "Data Operations"

## Expressions

Convert types
Perform simple calculations/date/time
Generate data (current date, GUID,random num)
Handling optional values
"IF" conditional statements 
Working with lists

Can edit Dynamic Content with Expressions.

````
myid: 123
mytitle: This item is due at <time>    ---->  This item is due at 2017-09-26T19:00:00Z
myname: Stephen

Step 1 - expression name
replace()

replace(textToSearch, textToFind, textToReplace)

replace($text, '<text>', $date)

replace(body('Get_record')['mytitle'], '<text>', utcnow())
````

## Data Types

Text *aka Strings*
Normal - 'example string'
Email,URL,phone, etc..

Non-text
Numbers, Booleans, Arrays, objects, XML content

There are a bunch of conversions functions for data types. Most of the time, it's done automatically but you may need to write an expression that does explicity conversion.

### Working with Strings

`concat()` - strings together

### Arithmetic
Cannot type it directly into the function expression language. Have to type add(a+b)... x + Y * Z ---> add(X,mul(Y,Z))

### Date / Time
`addToTime()`
`convertTimeZone()`
`formatDateTime()`
`dayOfWeek()`

### Expressions in conditions
`equals(object1, object2)`
`and(ex1, ex2)`
`or(ex1, ex2)`

### if() expressions

`if ($condition, $conditionTrue, $conditionFalse)`

Can only determine whether or not input in a field is defined.


### Handling optional values
Use the `?` character after selecting a property
Then, use the `coalesce()` function

`coalesce(body('Get_record')?['content'], 'Default Value')`


## Demos

### Working with Arrays

Ways to work with arrays ---
Repeat an action over each list item
Get a single item from a list
Filter a list down
Make a list work with a different action

`['Jane', 'Dan', 'Steve']`

