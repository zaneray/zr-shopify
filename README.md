# ZR Shopify Base

This project acts as the base starter theme for all ZaneRay Shopify projects. Follow the steps below to create a new Shopify theme using this as a starter theme.
Please refer to the official Shopify [Slate Docs](https://github.com/Shopify/slate/wiki/Getting-Started) for a full development reference.

## System Requirements

- **Node:** The current Long-Term Support version (LTS), greater than 6.0
- **NPM 5+:** Make sure your version of [NPM](https://www.npmjs.com/get-npm) is up to date.
- **Shopify Slate Toolkit:** Use NPM to install Shopify/slate globally
```
$ npm install -g @shopify/slate
```

## Create Your New Theme

To create a new Shopify theme based off of this starter template, run the following in your terminal:

```
$ npx create-slate-theme your-theme-name zaneray/zr-shopify
```

Where "your-theme-name" is the name of your new theme, and "zaneray/zr-shopify" points directly to this theme repository in github.

## Connect To Your Store

The ZR Shopify Base theme is connected by default to the ZaneRay Bootstrap Store. Before doing any development on your new theme, please connect it to your own Shopify store.

[Follow these steps](https://github.com/Shopify/slate/wiki/3.-Connect-to-your-store) to modify your **.env** file and connect your store to your theme.

## Start developing your new theme

Thats it! To start development, run the following command from a terminal in your new theme directory:

```
npm start
```

Your static development assets (css, js, etc.) will be served from a local express server running at https://localhost:8080.

You will need to visit [https://localhost:8080](https://localhost:8080) in order to accept the privacy certificate so that you can receive your local dev assets.

[Full development reference](https://github.com/Shopify/slate/wiki/4.-Start-developing)

## ZR Shopify Theme Reference

The ZR Shopify Theme uses Bootstrap 4 as a base css framework and for certain JS components.  Please visit the [https://getbootstrap.com/docs/4.0/components/alerts/](Bootstrap 4 Docs) for official reference.

All Bootstrap JS components are organized in the **/src/assets/scripts/vendor/bootstrap/bootstrap.js** file.  They can then be imported from that file into any part of the project.  By default, the **theme.js** file imports the Bootstrap Modal, Scrollspy and Tooltip components globally.

The Bootstrap styles are pulled into the **/src/assets/styles/core/bootstrap.scss** file, with only certain component/framework styles enabled by default.  You can uncomment any other Bootstrap styles you need here, if they are not already enabled.  Bootstrap override variables and mixins are setup in the **/core/bootstrap-override** directory of styles.

