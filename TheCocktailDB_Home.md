# Table of Contents
* [The Cocktail DB API](#The-Cocktail-DB-API)
* [Rate Limits](#Rate-Limits)
* [Schema](#Schema)
    - [API calls that require a key](#API-calls-that-require-a-key)
    - [API calls that do not require a key](#API-calls-that-do-not-require-a-key)
* [Errors](#Errors)
* [Support](#Support)
* [Related Projects](#Related-Projects)
* [API Index](API-Index)

## The Cocktail DB API

[The Cocktail DB](https://www.thecocktaildb.com/) is an open, crowd-sourced database of drinks and cocktails from around the world. [The Cocktail DB](https://www.thecocktaildb.com/) provides an API for developers and other interested people to quickly find information about cocktails, ingredients and other cocktail related items and return the information in JSON format. 

Basic functionality of the API is free to use for development and educational purposes. A production key is required when publicly releasing an application and can be obtained by subscribing through Patreon at [The Cocktail DB Patreon Supporter](https://www.patreon.com/thedatadb) for $3.00 a month. 

The production key provides access to advanced features: multiple ingredient filters, latest images, random images, popular cocktails, and recently added cocktails. Additionally, the production key ([available through Patreon subscription](https://www.patreon.com/thedatadb)) allows query results of over 100 items. 

## Rate Limits

The free API key allows up to 100 results per query for most search calls. The production API key provides the full results of all search calls and allows the adding of new cocktails and images. To get a production API key  [Subscribe to The Cocktail DB through Patreon](https://www.patreon.com/thedatadb)

## Schema

### API calls that require a key

ht<span>tps://</span>www.thecocktaildb.com/api/json/v1/**_Your_API_Key_**\/**_API_Call_**\.php **_Required_Optional_Query_String_**

The **_bold and italicized_** items indicate values that must be changed and are as follows:
* **_Your_API_Key_**: The free or your production API key.
* **_API_Call_**: The name of the API call (e.g. search, list, lookup).
* **_Required_Optional_Query_String_**: If the API call requires a query it will be entered at the end of the call (see the individual API calls for more details). API calls that do not require queries will not require a query.

### API calls that do not require a key

Please refer to the individual API call for more details.

## Errors

| Error | Text | Description |
| --- | ---| --- |
| **403** | Forbidden | The server understands the request but will not authorize it. Verify your API call is well-formatted. |
| **404** | Not Found | The server cannot find the the requested page/data. Verify that the API call is valid.|
| **KEY** | None | The server processes the API call and returns a JSON string, but the key is not a production key. The returned JSON string will contain "Only For Patreon supporters sorry" and not provide the data you requested. Verify your production key and if needed get a subscription at [The Cocktail DB Patreon Supporter](https://www.patreon.com/thedatadb). |

## Support

### Email: [thedatadb@gmail.com](mailto:thedatadb@gmail.com) 
&emsp; _Please state if you are a Patreon Supporter_    

The API and site will always remain free to access at its basic level. If you love [The Cocktail DB](https://www.thecocktaildb.com/) and want new features, sign up as a [Patreon supporter](https://www.patreon.com/thedatadb) for $3.00 a month (cancel at any time). 

Your support pays for the servers bandwidth and development of new features and content. Membership allows connection to the TheDataDB Discord channel, newsletter, and release notes.

## Related Projects

<div align="center">

[![The Sports DB](https://www.thecocktaildb.com/images/logo-tsdb.png 'The Sports DB')](https://www.thesportsdb.com/) &emsp; [![The Audio DB](https://www.thecocktaildb.com/images/logo-tadb.png 'The Audio DB')](https://www.theaudiodb.com/) &emsp; [![The Meal DB](https://www.thecocktaildb.com/images/logo-tmdb.png 'The MealDB')](https://www.mealdb.com/)

</div>