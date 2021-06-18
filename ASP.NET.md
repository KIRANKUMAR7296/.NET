# ASP.NET 

<table>
  <tr>
    <td><a href='#app'>A. Application Life Cycle</a></td>
    <td><a href='#page'>B. Page Life Cycle</a></td>
    <td><a href='#state'>C. State Management</a></td>
  </tr>
</table>

<h3 anme='app'>A. Application Life Cycle</h3>

- When an `ASP.NET` Web Application is launched, Series of steps make a Life Cycle of the Application.

#### 1. Application Start 

- `User` makes a `Request` to the `Server`.
- `Variables` are set to there `Default` Values.

#### 2. Object Creation

- Creates `HttpContext` ( Container for Objects `Request` and `Response` informations )
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

<h3 anme='state'>C. State Management</h3>

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

### Validation Controls
 
Validation Control |	Description
:--- | :---
RequiredFieldValidation |	Makes an Input Control a required field ( Texbox with * )
CompareValidator |	Compares the value of one input control to the value of another input control or to a fixed value.
RangeValidator |	Checks that the user enters a value that falls between two values range.
RegularExpressionValidator |	Ensures that the value of an input control matches a specified Pattern ( Email Address, Mobile No, Pincode )
CustomValidator |	Allows you to write a method to handle the validation of the value entered.
ValidationSummary |	Displays a report of all validation errors occurred in a Web page.

### Page Life Cycle Stages

Stage | Description
:--- | :---
Page Request | ASP.NET Determines whether the User Requests a `Fresh` Page request or `Cache` Version.
Start | ASP.NET Determines whether the Request is `PostBack` or a `New Request`.
Initialization | Controls and Properties are set ( Dropdowns are filled ) 
Load | If Request is PostBack, Informations are recovered from View State and Control State.
Postback event handling | Validations are checked ( e.g. Whether Textbox are filled or not )
Rendering | Viewstate is saved for the Page and all controls.
Unload |  Page properties are unloaded and final cleanup is performed.

