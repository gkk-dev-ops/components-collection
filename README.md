# Daily UI designs
## Goal
Aim is to implement all designs from [Design daily](https://uidesigndaily.com/)

## Adding components
To add new one to the gallery you need to go to the `/src/App.vue`
register new component by appending `component` and `returned data`

```JS
export default {
  name: 'App',
  components: {
    GalleryItem,
    LoginForm,
    CreditCardCheckout,
    yourComponentName
    },
  data() {
    return {
        LoginForm: 'LoginForm',
        CreditCardCheckout: 'CreditCardCheckout',
        yourComponentName: 'yourComponentName'
    };
  }
};
```

Then push it to the gallery:
```JS
<GalleryItem
    title="yourComponentNameDesignDailyName"
    date="dateOfDesignCreation"
    dailyUILink="linkToComponentDesing">
    <component :is="yourComponentName"></component>
</GalleryItem>
```