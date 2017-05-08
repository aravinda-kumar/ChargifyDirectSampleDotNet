Chargify Direct Sample .NET
==========================

This is a small [ASP.NET MVC](http://www.asp.net/mvc) app that demonstrates how to use [Chargify Direct](http://docs.chargify.com/chargify-direct-introduction) for
Signups. It leverages the .NET [Chargify2](https://github.com/kfrancis/Chargify2) library to create the Direct secure form inputs and signature, verify the redirect 
response, and fetch the call response.

Getting Started
---------------

1. Clone this repo to your local machine
2. Edit `web.config` to add your own API User credentials (created on your site, https://your-subdomain.chargify.com/settings#chargify-direct)
3. Create products on your API User's Site with handles 'basic' and 'premium' (or edit the example to match product handles you have)
4. Remove the https global filter (if applicable)
5. Run the app

Features
---------------

1. Uses the transparent redirect to post sensitive data directly to Chargify
2. Uses the Call API endpoint to fetch information to display a receipt

##Demo##
This code has been deployed [here](https://chargify-direct-sample.azurewebsites.net) for your convenience, so you can create test subscriptions.

You can try a sample live update endpoint [here](https://chargify-direct-sample.azurewebsites.net/Home/Update/17723461).

For v1 API access, try the [Chargify.NET wrapper](http://chargify.codeplex.com).