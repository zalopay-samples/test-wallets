# Test wallets

- [Test wallets](#test-wallets)
  - [Overview](#overview)
  - [Installation](#installation)
  - [Registration](#registration)
  - [Deposit](#deposit)
  - [Questions](#questions)

## Overview

This repository contains ZaloPay pre-built binaries for mobile platforms (iOS, Android)

## Installation

Click/tap on the following button to install

<!-->remove iframe because of limitation on downloading build on Safari<-->
<style>
  .container {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    width: 100%;
  }
  .cta {
    border-radius: 10px;
    border: none;
    cursor: pointer;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI',
      Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue',
      sans-serif;
    color: white;
    line-height: 24px;
    padding: 8px 16px;
    width: fit-content;
  }
  .ios {
    background-color: rgb(142, 142, 147);
    margin-right: 16px;
  }
  .android {
    background-color: rgb(50, 222, 133);
  }
  .title {
    margin: 0 !important;
    font-size: 18px;
    font-weight: 500;
  }
  .subtitle {
    margin: 0 !important;
    font-size: 12px;
  }
</style>

<br />
<div class="container">
  <div align="center">
    <a
      href="itms-services://?action=download-manifest&url=https://github.com/zalopay-samples/test-wallets/raw/main/ios/8.25.0/manifest-8.25.0.plist"
      style="text-decoration: none"
    >
      <div class="cta ios">
        <img
          src="./images/icons/apple.svg"
          width="32"
          height="32"
          style="margin-right: 8px"
          alt="iOS Logo"
        />
        <div>
          <p class="title">8.25.0 Current</p>
          <p class="subtitle">Latest Features</p>
        </div>
      </div>
    </a>
  </div>
  <div align="center">
    <a
      href="https://github.com/zalopay-samples/test-wallets/raw/main/android/ZaloPay_Android_8.25.0.apk"
      style="text-decoration: none"
    >
      <div class="cta android">
        <img
          src="./images/icons/android.svg"
          width="32"
          height="32"
          style="margin-right: 8px"
          alt="Android Logo"
        />
        <div>
          <p class="title">8.25.0 Current</p>
          <p class="subtitle">Latest Features</p>
        </div>
      </div>
    </a>
  </div>
</div>
<br />


Other downloads:

| Platform | ZaloPay Version | Updated Date | Download URL |
| -------- | --------------- | ------------ | ------------ |
| iOS      | 7.23.0          | 03/10/2022   | [ZaloPay_iOS_7.23.0.ipa](itms-services://?action=download-manifest&url=https://github.com/zalopay-samples/test-wallets/raw/main/ios/7.23.0/manifest-7.23.0.plist) |
| Android  | 7.20.0          | 03/10/2022   | [ZaloPay_Android_7.20.0.apk](https://github.com/zalopay-samples/test-wallets/raw/main/android/ZaloPay_Android_7.20.0.apk) |

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

<iframe src="html/cashin.html" width="100%" height="350px" style="background: transparent; border: none;">
  <p>Your browser does not support iframes.</p>
</iframe>

## Questions

If you have any question, feel free to [discuss](https://github.com/zalopay-samples/test-wallets/discussions)
