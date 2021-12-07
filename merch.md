---
layout: page
title: merch
permalink: /merch/
---
<!-- TODO: Stop sale after set date -->
{% assign day = page.date | date: "%-d"  %}
{{day}}
{% assign sale_active = false %}
{% if sale_active %}<h2 style="color:darkred; text-align: center; font-weight: bold;">BLACK FRIDAY SALE UNTIL DEC 3RD</h2>{% endif %}

<div class="flex w100">
  <img class="col-md-6 fix-height" src="/img/merch1-1.jpg">
  <img class="col-md-6 fix-height" src="/img/merch1-2.jpg">
</div>

<div id="container-product1" class="bg-white p20">
  <h2>'Heaven' Tee{% if sale_active %} <span style="color: darkred;">BLACK FRIDAY SALE</span>{% endif %}</h2>
  <h2 class="mb0">{% if sale_active %}<span style="text-decoration: line-through;">$35</span> $25{% else %}$35{% endif %}<small>USD</small></h2>
  <h4>+ $10 shipping</h4>
  <p>Orders begin shipping early December</p>
  <form target="paypal" action="https://www.paypal.com/cgi-bin/webscr" method="post">
    <input type="hidden" name="cmd" value="_s-xclick">
    <input type="hidden" name="hosted_button_id" value="R53UC2CPD99D2">
    <table>
    <tr><td><input type="hidden" name="on0" value="Sizes">Sizes</td></tr><tr><td><select name="os0">
      <option value="XL">XL </option>
      <option value="Large">Large </option>
      <option value="Medium">Medium </option>
      <option value="Small">Small </option>
    </select> </td></tr>
    </table>
    <input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_cart_LG.gif" border="0" name="submit" alt="PayPal - The safer, easier way to pay online!">
    <img alt="" border="0" src="https://www.paypalobjects.com/en_US/i/scr/pixel.gif" width="1" height="1">
  </form>
</div>

<div class="flex w100">
  <img class="col-md-6 fix-height" src="/img/merch2-1.jpg">
  <img class="col-md-6 fix-height" src="/img/merch2-2.jpg">
</div>

<div id="container-product2" class="bg-white p20">
  <h2>'Heaven' Hoodie{% if sale_active %} <span style="color: darkred;">BLACK FRIDAY SALE</span>{% endif %}</h2>
  <h2 class="mb0">{% if sale_active %}<span style="text-decoration: line-through;">$55</span> $35{% else %}$55{% endif %}<small>USD</small></h2>
  <h4>+ $10 shipping</h4>
  <p>Orders begin shipping early December</p>
  <form target="paypal" action="https://www.paypal.com/cgi-bin/webscr" method="post">
    <input type="hidden" name="cmd" value="_s-xclick">
    <input type="hidden" name="hosted_button_id" value="RUY2FXJRBGCVU">
    <table>
    <tr><td><input type="hidden" name="on0" value="Sizes">Sizes</td></tr><tr><td><select name="os0">
      <option value="XL">XL </option>
      <option value="Large">Large </option>
      <option value="Medium">Medium </option>
      <option value="Small">Small </option>
    </select> </td></tr>
    </table>
    <input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_cart_LG.gif" border="0" name="submit" alt="PayPal - The safer, easier way to pay online!">
    <img alt="" border="0" src="https://www.paypalobjects.com/en_US/i/scr/pixel.gif" width="1" height="1">
  </form>
</div>