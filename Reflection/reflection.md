# Reflection

## Question 1 (50 words)
#### When and why should you use a function like `carefulSubract` rather than `subtract`? 

carefulSubtract and subtract are essentially the same functions. However, naming functions differently, especially if you're using two subtracts can be helpful. It can remind you of the function's purpose. Or it can provide information to those viewing the code. subtract implies a simple subtraction function. In contrast, carefulSubtract denotes conditions.

## Question 2 (100 words)
#### What are `data types`, and how does data typing work in JavaScript? Name at least 4 built-in data JS data types. 
'Data types' are the information in the code that signify the type of information that can be stored and changed. 
The six main ones fall under three classifications: primitive/primary, composite/reference and special. Primary/primitive data types include strings, numbers and booleans. Composite/reference data types encompass objects, arrays and functions. Secial data types include undefined and null.
Data types tells JavaScript how to treat different pieces of information. JavaScript treats data differently depending on its data type. Examples of built in data types include null, undefuned, boolean, number and string.
Source 1: https://www.tutorialrepublic.com/javascript-tutorial/javascript-data-types.php#:~:text=Data%20Types%20in%20JavaScript,and%20manipulated%20within%20a%20program.&text=String%2C%20Number%2C%20and%20Boolean%20are,objects)%20are%20composite%20data%20types.
Source 2: https://medium.com/@shobhitsingh29/understanding-js-data-types-1ac8977ac8ae
Source 3: https://www.oreilly.com/library/view/you-dont-know/9781491905159/ch01.html#:~:text=Review,the%20values%20in%20them%20do.

## Question 3 (100 words)
#### What is the advantage to storing information as an object (`{firstName: 'Italo', lastName: 'Calvino', profession: 'novelist' }`) rather than as an array (`['Italo', 'Calvino', 'novelist']`)? Are there any disadvantages?
Objects and arrays are both similar ways of storing information. The difference between objects and arrays is the indexing. An object is an unordered collection of information. In contrast, an array is ordered. We use arrays when the order of the information matters. If the order doesn't matter, we can use an object. The advantage to using an array is being able to analyze the information such as word length. The disadvantage is the difficulty in pulling up specific words. In contrast, an advantage of objects is being able to quickly and easily find specific words. The disadvantage is that it does not allow for more complex analyses, unlike an array.
Source: https://forum.freecodecamp.org/t/best-practice-objects-vs-arrays/179358/3

## Question 4 (150 words)
#### The function `sentences` transforms a data structure (in this case, a list of object literals) into a sequence of sentences. If the data structure were less predictable (e.g., if some properties of each object were occasionally missing, or if their data type was not always the same), what programming techniques could you use to ensure that your function produced a coherent output? Also, can you think of a more interesting "transform" that could be done with the same data structure?
The programming techniques Object(values) or object.entries can be used to ensure the function has a coherent output. Object(values) provides arrays of the object's property values in the order of the "for... in loop." Even though the data structure is unpredictable, object(values) orders the properties as if I was manually looping. Similarly, object.entries() will return arrays of the objects enumerable properties. Specifically, the enumerable properties [key, value]. Object.entries() also returns the array in the same order of the "for... in" loop. This data structure could also be used to build a generator that returns random object literals. Additionally, another use of the data structure is randomly filling in a Mad Libs style story or paragraph with the objects.
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_objects/Object/values
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/entries 