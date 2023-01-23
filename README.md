# Daily UI designs
## Goal
Aim is to implement all designs from [Design daily](https://uidesigndaily.com/)

## Adding components
To add new one to the gallery you need to go to the `/src/App.vue`
register new component by appending `component`.

```JS
export default {
  name: 'App',
  components: {
    GalleryItem,
    LoginForm,
    CreditCardCheckout,
    yourComponentName
    }
};
```

Then push it to the gallery:
```JS
<GalleryItem
    title="yourComponentNameDesignDailyName"
    date="dateOfDesignCreation"
    dailyUILink="linkToComponentDesing">
    <yourComponent/>
</GalleryItem>
```