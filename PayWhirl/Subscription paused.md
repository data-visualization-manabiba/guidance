# New subscription


## Email subject

[{{ shop_name }}] Your subscription has been paused

## Email body (HTML)

<!DOCTYPE html>
<html>

<head>
  <meta http-equiv="Content-Security-Policy" content="script-src 'none'; style-src * 'unsafe-inline'; default-src *; img-src * data:">
  <title>{{ subject }}</title>
  <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
  <meta name="viewport" content="width=device-width">
  <style>
    body{margin:0;}
    table.body{border-collapse:collapse;border-spacing:0;height:100%!important;width:100%!important;}
    table{border-collapse:collapse;border-spacing:0;}
    table.row{width:100%;}
    table.actions{margin-top:20px;}
    td{font-family:-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;}
    h1 a{color:#333;font-size:30px;text-decoration:none;}
    h1 a:hover,h1 a:active,h1 a:visited{color:#333;font-size:30px;}
    h2{font-size:24px;font-weight:400;margin:0 0 10px;}
    a:hover,a:active,a:visited{color:#1990C6;text-decoration:none;}
    .header{margin:40px 0 20px;}
    .content__cell{padding-bottom:40px;}
    .content__cell p{color:#777;font-size:16px;line-height:150%;margin:0;}
    .footer{border-top-color:#e5e5e5;border-top-style:solid;border-top-width:1px;}
    .footer__cell{padding:35px 0;}
    .container{margin:0 auto;text-align:left;width:560px;}
    .link__cell a{color:#1990C6;font-size:16px;text-decoration:none;}
    .button__cell{border-radius:4px;}
    .button__text{color:#fff;display:block;font-size:16px;padding:20px 25px;text-decoration:none;}
    .button__text:hover,.button__text:active,.button__text:visited{color:#fff;text-decoration:none;}
    .empty-line{line-height:.5em;}
    .main-action-cell{float:left;margin-right:15px;}
    .secondary-action-cell{margin-top:19px;}
    .shop-name__text{color:#333;font-size:30px;font-weight:400;margin:0;}
    .subscription-id__cell{color:#999;font-size:16px;text-transform:uppercase;}
    .disclaimer__subtext{color:#999;font-size:14px;line-height:150%;margin:0;}
    .disclaimer__subtext a{color:#1990C6;font-size:14px;text-decoration:none;}
    @media (max-width: 600px) {
      .container{width:94%!important;}
      .main-action-cell{float:none!important;margin-right:0!important;}
      .secondary-action-cell{text-align:center;width:100%;}
      .header{margin-bottom:2px!important;margin-top:20px!important;}
      .shop-name__cell{display:block;}
      .subscription-id__cell{display:block;margin-top:20px;}
      .button{width:100%;}
    }
  </style>
</head>

<body>
  <table class="body"><tr><td>
    <table class="header row"><tr><td class="header__cell"><center>
      <table class="container"><tr><td>
        <table class="row"><tr>
          <td class="shop-name__cell">
            <h1 class="shop-name__text">
              <a href="{{ shop_link }}">{{ shop_name }}</a>
            </h1>
          </td>
          <td class="subscription-id__cell">Subscription #{{ subscription_id }}</td>
        </tr></table>
      </td></tr></table>
    </center></td></tr></table>

    <table class="row content"><tr><td class="content__cell"><center>
      <table class="container"><tr><td>
        <h2>Your subscription has been paused</h2>
        <table class="row actions"><tr><td class="actions__cell">
          <table class="button main-action-cell"><tr>
            <table class="row actions">
              <tr>
                <td class="empty-line"> </td>
              </tr>
              <tr>
                <td class="actions__cell">
                  <table class="button main-action-cell"><tr><td class="button__cell" align="center" bgcolor="#1990C6">
                    <a href="{{ subscription_link }}" class="button__text">Manage your subscription</a>
                  </td></tr></table>
                  <table class="link secondary-action-cell"><tr>
                    <td class="link__cell">or <a href="{{ shop_link }}">Visit our store</a></td>
                  </tr></table>
                </td>
              </tr>
            </table>
          </tr></table>
        </td></tr></table>
      </td></tr></table>
    </center></td></tr></table>
    <table class="row footer"><tr><td class="footer__cell"><center>
      <table class="container"><tr><td>
        <p class="disclaimer__subtext">
          If you have any questions, reply to this email or contact us at
          <a href="mailto:{{ contact_email }}">{{ contact_email }}</a></p>
      </td></tr></table>
    </center></td></tr></table>
  </td></tr></table>
</body>

</html>
