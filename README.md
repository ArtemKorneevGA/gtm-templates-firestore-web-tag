# The Web GTM TAG for Firestore

![The Web GTM Tag for Firestore.](https://gtm-gear.com/images/2022/04/firestore/firestore-tag.png)

## Description

The **Firestore Web Tag** template allows you to create a list of the rules on how to change the user property. For example, you can create a tag which will be fired on the purchase trigger and have these rules: increase transactions by one, increase revenue on purchase amount, set last purchase date to current date.

## Set Up

- Follow on instructions on how to set up [Firestore Server Client](https://github.com/ArtemKorneevGA/gtm-templates-firestore-server-client);
- Follow on instructions on how to set up [Firestore Server Tag](https://github.com/ArtemKorneevGA/gtm-templates-firestore-server-tag);
- Download the **Firestore Web Tag** template.tpl file from this GitHub repo;
- In your Web container go to the Templates page, in Tags Template section click the New button;
- Open the top right menu and click on Import;
- Select **template.tpl** file, and click save;
- Close the Template Editor window;
- Go to the Tags page. Click on the New button and select **Firestore Web Tag**;
- Name your tag, for example **firestore**;
- Set the Server-Side GTM URL;
- Set the User Key field, in production in can be **user_token** or **user_id**;
- Add rules, for each rule set action type, value, and returning value;
- Checkbox «Set cookie after user properties will be updated» is selected by default. But if you don’t need changed user property on the front-end, you can uncheck it;
- In the «DataLayer settings» you can change DataLayer Event Name this is the name of a dataLayer event pushed after the user state will be updated;
- Set the «Event Type» value. If you have a few Firestore Tags, for example one for registration, one for purchase, this value will help you to make triggers only for specific **firestore_updated** dataLayer events.
