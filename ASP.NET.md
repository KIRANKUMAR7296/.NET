# ASP.NET 

### State Management
- `Maintain` and `Store` the Information of any User till the end of the `User Session`.

<table>
  <tr><th colspan=2>State Management</th></tr>
  <tr><th>Server Side</th><th>Client Side</th></tr>
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
