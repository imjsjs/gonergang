---
layout: page
title: merch
permalink: /merch/
---

![merch1](/img/merch1.jpg)

<div id="smart-button-container" class="bg-white p20">
  <h2>'Heaven' Tee (Presale)</h2>
  <h2>$30<small>USD</small></h2>
  <p>Orders begin shipping early December</p>
  <div style="text-align: center;">
    <div id="paypal-button-container"></div>
  </div>
</div>
<script src="https://www.paypal.com/sdk/js?client-id=sb&enable-funding=venmo&currency=USD"
  data-sdk-integration-source="button-factory"></script>
<script>
  function initPayPalButton() {
    paypal.Buttons({
      style: {
        shape: 'pill',
        color: 'blue',
        layout: 'vertical',
        label: 'buynow',

      },

      createOrder: function (data, actions) {
        return actions.order.create({
          purchase_units: [{
            "description": "GONER “They watched me go to heaven” limited edition T-Shirt.\nWhite printed on black Tee. ",
            "amount": {
              "currency_code": "USD",
              "value": 43,
              "breakdown": {
                "item_total": {
                  "currency_code": "USD",
                  "value": 35
                },
                "shipping": {
                  "currency_code": "USD",
                  "value": 8
                },
                "tax_total": {
                  "currency_code": "USD",
                  "value": 0
                }
              }
            }
          }]
        });
      },

      onApprove: function (data, actions) {
        return actions.order.capture().then(function (orderData) {

          // Full available details
          console.log('Capture result', orderData, JSON.stringify(orderData, null, 2));

          // Show a success message within this page, e.g.
          const element = document.getElementById('paypal-button-container');
          element.innerHTML = '';
          element.innerHTML = '<h3>Thank you for your payment!</h3>';

          // Or go to another URL:  actions.redirect('thank_you.html');

        });
      },

      onError: function (err) {
        console.log(err);
      }
    }).render('#paypal-button-container');
  }
  initPayPalButton();
</script>