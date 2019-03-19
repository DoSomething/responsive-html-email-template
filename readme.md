Our default Customer.io email template, forked from http://leemunroe.github.io/responsive-html-email-template/email.html.

## Usage

To include a Call To Action button within the email content:

```
<table role="presentation" border="0" cellpadding="0" cellspacing="0" class="btn btn-primary">
  <tbody>
    <tr>
      <td align="center">
        <table role="presentation" border="0" cellpadding="0" cellspacing="0">
          <tbody>
            <tr>
              <td>
                <a href="{{event.actionUrl}}" target="_blank">
                  Join The Movement
                </a>
              </td>
            </tr>
          </tbody>
        </table>
      </td>
    </tr>
  </tbody>
</table>
```
