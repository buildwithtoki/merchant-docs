# 😆 Hiding the Wallet

If you do not want the wallet to show until a user clicks on your customer account icon (or button)..

1. Toggle the wallet off on your theme
2. Add this code to the icon or button

```
<a href="javascript:tokiWallet.request({ method: 'toki_open_popup', params: {} })">
```

