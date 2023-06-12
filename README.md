# Suppliers-Extra-Validation

This automation adds some extra-validation on to an existing website. The "number of employees" is checked to be an actual number, and the address is being validated using an external validation API.

How to demo:

1. Updete the "HTTP Request" activity's Request URL to add your own google api key. The activiti is in the "on open check address.xaml" file.
2. Open https://www.rpasamples.com/suppliers in chrome
3. Run the automation
4. Click on "New Supplier"
5. Write something in the internal / external name fields
6. Write something like "lots of them" for the # of employees
7. Write an address that is not 100% correct, and only use the 1st address field (ex: don't put in the zip code)
8. Click "save". You will see that it asks you to enter a number for the # of employees. Enter a number.
9. Click "save" again. You will see that it will validate the address and propose another (fixed) address to be used.

And you're done.
