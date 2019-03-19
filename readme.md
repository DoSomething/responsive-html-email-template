The DoSomething.org email template to use for Customer.io emails, forked from http://leemunroe.github.io/responsive-html-email-template/email.html.

## Contributing

Our default Customer.io email layout should be the same as the `email.html` in this project.

To deploy a new release, copy paste the new `email.html` content into our default Email Template in Customer.io :scissors: :art:

## Usage

To add a Call To Action button:

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
