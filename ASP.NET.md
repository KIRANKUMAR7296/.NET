# ASP.NET 

<table>
  <tr>
    <td><a href='#page'>Page Life Cycle</a></td>
    <td><a href='#state'>State Management</a></td>
    <td><a href='#valid'>Validation Controls</a></td>
    <td><a href='#client'>Client Side and Server Side Controls</a></td>
  </tr>
</table>

<h3 anme='app'>A. Application Life Cycle</h3>

- When an `ASP.NET` Web Application is launched, Series of steps make a Life Cycle of the Application.

#### 1. Application Start 

- `User` makes a `Request` to the `Server`.
- `Variables` are set to there `Default` Values.

#### 2. Object Creation

- Creates `HttpContext` ( Container for `Request` and `Response` Objects )
- `HttpRequest` ( Contains Information about the `Current` Request made by Client to the Server )
- `HttpResponse` ( Contains Response that is sent by Server to the Client )

#### 3. HttpApplication Creation

- `Object` is Created by Server for each Request.
- e.g. User requests for Websites of `Flipkart` and `Amazon` to the Server.
- `Server` creates two Web Application `Objects`, one for Flipkart and one for Amazon.

#### 4. Dispose 
- Manually `Release` the Resources.

#### 5. Application End 
- Web Application is `unloaded` from Memory.

<h3 name='page'>B. Page Life Cycle</h3>

- When an ASP.NET Page is called it goes through Series of Life Cycle, before Server `Response` to User.

#### 1. Page Request 

- When User requests for Page fom Server, Server checks if the request is First time or not.
- If Request is for `First` time, Page is compiled and responded to User.
- If Request is not for First time, Cache is checked whether Page exists there and then Sent to User.

#### 2. Page Start

- Create `Request` and `Response` Objects. 
- `Request` Objects : Hold all information which was sent by User at the time of request to Server.
- `Response` Object : Hold all information which is sent back to User by Server.

#### 3. Page Initialization

- All the controls ( Label, Textbox, Dropdown ) on web page are initialized.

#### 4. Page Load

- Page loads with `Default` Values.
- e.g. Fill Dropdowns or If Textbox has default value that is filled.

#### 5. Validation

- `Check` for Validation and Load Error if Validation Conditions are not Satisifed.

#### 6. PostBack Event Handling 

- Event is Triggered if Same Page is Loaded again.
- Response to some earlier event ( e.g. If you click on submit button same page is loaded with Message )

#### 7. PostBack Rendering 

- All the Information on the Page is `Saved`and Result is sent to User as a Web Page.

#### 8. Unload

- Removing all unwanted `Objects` from Memory.

<h3 name='state'>C. State Management</h3>

- `Maintain` and `Store` the Information of any User till the end of the `User Session`.
- Browser communicates with Server using `HTTP` or `HTTPs` Protocol.
- Browsers are `Stateless` ( Once the Browser is closed it do not keep the State of `Websites` and `URLs` )
- When we reopen the Browser we enter the URL again.

> State Informations like User Identity, Objects, Allocated Memory and Session ID.

<table>
  <tr><th colspan=2>State Management Types</th></tr>
  <tr><th>Server Side</th><th>Client Side</th></tr>
  <tr><th>Information is stored in User Memory</th><th>State information is stored on Client Side</th></tr>
  <tr>
    <td>
      <ul>
        <li>Session ( Stores Information and Identity )</li>
        <li>Application ( Stores User Activity )</li>
        <li>Cache ( Stores Data in CPU Memory )</li>
      </ul>
    </td>    
    <td>
      <ul>
        <li>Cookies ( Stores User Information, Session and Application )</li>
        <li>Viewstate ( Stores any type of Data temporarily after a PostBack )</li>
        <li>Controlstate</li> ( Enables the Property of Viewstate )
        <li>Query String ( Stores the value in URL, Visible to all Users. )</li>
        <li>Hidden Field ( Stores value that are not displayed on Browser )</li>
      </ul>
    </td>    
  </tr>
</table>

<h3 name='valid'>Validation Controls</h3>
 
Validation Control |	Description
:--- | :---
RequiredFieldValidation |	Makes an Input Control a required field ( Texbox with * )
CompareValidator |	Compares the value of one input control to the value of another input control or to a fixed value.
RangeValidator |	Checks that the user enters a value that falls between two values range.
RegularExpressionValidator |	Ensures that the value of an input control matches a specified Pattern ( Email Address, Mobile No, Pincode )
CustomValidator |	Allows you to write a method to handle the validation of the value entered.
ValidationSummary |	Displays a report of all validation errors occurred in a Web page.


<h3 name='client'>Client Side and Server Side Controls</h3>

- Controls are small Building Blocks of Graphical User Interface `GUI`. 

#### Client Side Controls 

1. `Button` Control : Button (Text Button), Link Button (Hyperlinks), Image Button (Button with Icon)
2. `Textbox` Control : Accept Input from User.
3. `Labels` : Display Texts (It can be changed based on execution condition)
4. `Check Box : Displays a Single Option that a User can Check or Uncheck.
5. `Radio` Button : Present a Group of Options from which User can select One.
6. `Radio` Button List and `Check` Box List : List Item Collections.
7. `Bulleted` List : Unordered Collection. 
8. `Numbered` List : Ordered Collection. 
9. `Hyperlink` Control : Similar to HTML \<a> Tag.
10. `Image` Control : Display Image, Similar to HTML \<img> Tag. 

#### Server Side Controls 

1. `Validation` Controls : Validate User Input
2. `Data Source` Controls : Data bindings to different Data Sources.
3. `Data View` Controls : Bind to Data from Data Source for Displaying.
4. `Personalized` Controls : Personalization of User Information on the Page.
5. `Login` and `Security` Controls : Provides Authentication (UserName and Pwd) and Authorization (Check for Permission)
6. `Master` Pages : Provide Consistent Layout and Interface throughout the Webpage.
7. `Navigation` Controls : Menu, NavBar, Tabs (Home, Contact, Career, About Us)
8. `Rich` Controls : Special Features (FileUpload, Calender Control, Range Selector)

Controls provides various features for Error Free Coding.
- Dragging and Droppig of Controls in Design View.
- Intellisense features to display methods and functions + Autocomplete.
- Property Windows to set the Property Values directly.
