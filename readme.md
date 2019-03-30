The DoSomething.org email template to use for Customer.io emails, forked from http://leemunroe.github.io/responsive-html-email-template per [recommendation by Customer.io](https://customer.io/docs/4-email-design-resources).

This email template contains `<style>` tags -- [Customer.io adds the styles inline to the email before it is sent](https://customer.io/docs/disable-premailer). 


## Contributing

Our default Customer.io email layout should be the same as the `email.html` in this project.

To deploy a new release, copy paste the new `email.html` content into our default [Email Template in Customer.io](http://docs.dosomething.org/customer-io#email-layouts) :scissors: :art:


## Usage

Here is example HTML to add into the Code Editor of an Email Workflow step:

```
<h1>Hello!</h1>
<p>
  You are receiving this email because you need to set a password to activate your DoSomething.org account. Here is the link to set your password:
</p>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" class="btn btn-primary content-blcok">
  <tbody>
    <tr>
      <td align="center">
        <table role="presentation" border="0" cellpadding="0" cellspacing="0">
          <tbody>
            <tr>
              <td> <a href="{{event.actionUrl}}" target="_blank">Reset Password</a> </td>
            </tr>
          </tbody>
        </table>
      </td>
    </tr>
  </tbody>
</table>
<p>
  This link will expire in 24 hours. Once you click the button above, you will be asked to reset your password on the page.
</p>
<p>
   If you have further questions, please reach out to help@dosomething.org. 
</p>
<hr>
<small>
  If you’re having trouble clicking the "Reset Password" button, copy and paste the URL below
into your web browser: {{event.actionUrl}}
</small>

```

### Buttons

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
