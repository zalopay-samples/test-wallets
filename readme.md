# Test wallets

- [Test wallets](#test-wallets)
  - [Overview](#overview)
  - [Installation](#installation)
  - [Registration](#registration)
  - [Deposit](#deposit)
  - [Questions](#questions)

## Overview

This repository contains ZaloPay pre-built binaries for mobile platforms (iOs, Android)

## Installation

Click/tap on the following button to install

<style>
  .cta {
        border-radius: 10px;
        border: none;
        cursor: pointer;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
</style>

<br />
<p align="center">
  <a href="itms-services://?action=download-manifest&amp;url=https://github.com/zalopay-samples/test-wallets/raw/main/ios/manifest.plist">
    <img src="https://img.shields.io/badge/-for%20iOS-gray?style=flat-square&logo=apple" height="60" class="cta" />
  </a>
</p>
<p align="center">
  <br />
  <a href="https://github.com/zalopay-samples/test-wallets/raw/main/android/zalopay-7.20.0.apk">
  <img src="https://img.shields.io/badge/-for%20Android-blue?style=flat-square&logo=android&logoColor=white" height="60" class="cta" />
  </a>
</p>
<br />

For iOS, once the installation is successful, you should trust ZaloPay app via settings in  `Device Management`

<p align="center">
  <img src="images/usage/ios-trust.png" width="240" />
</p>

Please consult [Install custom enterprise apps on iOS](https://support.apple.com/en-us/HT204460) for more information.

## Registration

<style>
  .step {
    background-color: transparent !important;
  }
</style>
**Step 1**: Open the ZaloPay app and log in using your Zalo account or mobile number.

Note: One phone number can only be linked to a single ZaloPay sandbox account.

<p align="center">
  <img src="images/usage/step-01.png" width="360" class="step"/>
</p>

**Step 2**: Enter the phone number and continue

<p align="center">
  <img src="images/usage/step-02.png" width="360" class="step"/>
</p>

**Step 3**: Enter the verification code of `111111` and continue with password setup

<p align="center">
  <img src="images/usage/step-03.png" width="360" class="step"/>
</p>

<br/>

## Deposit

To pay with ZaloPay Sandbox, you first have to deposit some money

<style>
  body {
    background-color: #f9f9f9;
    font-family: Arial, sans-serif;
  }
  .container {
    max-width: 500px;
    margin: 0 auto;
    padding: 20px;
    background-color: #fff;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
  h1 {
    font-size: 28px;
    font-weight: bold;
    margin-bottom: 20px;
  }
  form label {
    display: block;
    font-weight: bold;
    margin-bottom: 10px;
  }
  form input[type="tel"] {
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 10px;
    width: 95%;
    margin-bottom: 20px;
  }
  .g-recaptcha {
    margin-bottom: r120px;
  }
  form input[type="submit"] {
    background-color: #007bff;
    color: #fff;
    padding: 10px 20px;
    border-radius: 10px;
    border: none;
    cursor: pointer;
    transition: all 0.3s ease-in-out;
  }
  form input[type="submit"]:hover {
    background-color: #0062cc;
  }
</style>
<br />
<script src="https://www.google.com/recaptcha/enterprise.js?render=6Leii_glAAAAAOQKbY4LZEtwxitRiXFbNzvZgkJA"></script>
<script>
grecaptcha.enterprise.ready(function() {
    grecaptcha.enterprise.execute('6Leii_glAAAAAOQKbY4LZEtwxitRiXFbNzvZgkJA', {action: 'login'}).then(function(token) {
       // tbd
    });
});
</script>
<div class="container">
  <form method="get" action="https://zlpdev-mi-zlpdemo.zalopay.vn/zlp-demo/api/cashin">
    <label for="phone">Enter the registered phone number</label>
    <input type="tel" id="phone" name="phone" maxlength="15" pattern="[0-9]+" required>
    <div class="g-recaptcha" data-sitekey="6Leii_glAAAAAOQKbY4LZEtwxitRiXFbNzvZgkJA"></div>
    <input type="submit" value="Submit">
  </form>
</div>
<br />

## Questions

If you have any question, feel free to [discuss](https://github.com/zalopay-samples/test-wallets/discussions)
