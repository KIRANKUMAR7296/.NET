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
