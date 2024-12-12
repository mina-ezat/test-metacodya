# metacodya NPM Package

Npm package created to supply reusable components to metacodya developers.

## How to use it ?

Before installing package, you should have tailwindCSS installed and configured in your project as the package styling is built using tailwindCSS.

You should also include the index.css file of the package in the top of your app ( eg. in the top of App.tsx - your main file that contains the whole application - ) as following :

```javascript
import React from "react";

// The following import must be included to apply styles used
// in the package
import "../node_modules/metacodya/dist/index.css";

// This is an example for importing some components from package
import { SearchInput} from "metacodya";

function App() {
  return (
    <div className="container">
      <SearchInput setInputValue={(e) =>console.log(e)}  />
    </div>
  );
}
```

<section id="table">

## Table of components

<hr />
<ul id="table-contents">
      <li><a href="#user-content-UserInput">UserInput</a></li>
      <li><a href="#user-content-SearchInput">SearchInput</a></li>
</ul>
</section>
<hr />

## 🛠 Components included in the package :

<section id="UserNav">
 

### 9- UserInput

#### The UserInput takes same props as default input field with extra props :

- label ?
- labelStyle?: for styling label
- success ?: success message if validation is OK
- error ?: error message if there is a problem with validation
- onChangeFn ?: useState function to get change in value

```javascript
<UserInput label="Username" type={"text"} placeholder="type your username" />
<UserInput disabled label="Password" type={"password"} />
```

![App Screenshot](https://res.cloudinary.com/dvvmu40wx/image/upload/v1719683933/VODO/reusable%20components/InputField_ldixiy.png)

</section>

//=================================================

<a href="#user-content-table">Go back to the table of components</a>

//=================================================

<section id="Status">


### 13- SearchInput

#### The SearchInput takes 4 props :

- setInputValue : setState function to get the value of the input field
- disabled ?
- props ?: default input props
- className ?: addition TailwindCSS classes to apply

```javascript
<SearchInput setInputValue={setInputValue} disabled />
<SearchInput setInputValue={setInputValue}/>
```

![App Screenshot](https://res.cloudinary.com/dvvmu40wx/image/upload/v1719678813/VODO/reusable%20components/Search_input_e7gqzu.png)

</section>

//=================================================

<a href="#user-content-table">Go back to the table of components</a>

//=================================================

<section id="TextArea">

 

  
 
</section>
