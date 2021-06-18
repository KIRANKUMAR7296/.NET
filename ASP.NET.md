# ASP.NET 

### State Management
- `Maintain` and `Store` the Information of any User till the end of the `User Session`.
- Browser communicates with Server using `HTTP` or `HTTPs` Protocol.
- Browsers are `Stateless` ( Once the Browser is closed it do not keep the State of `Websites` and `URLs` )
- When we reopen the Browser we enter the URL again.

### State Informations
1. Objects 
2. Allocated Memory
3. Session ID

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
        <li>Viewstate ( Stores any type of Data used for Sending and Receiving Information. )</li>
        <li>Controlstate</li>
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

