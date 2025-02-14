# Manual Testing



{% hint style="info" %}
Make sure you've finished the installation guide and that **containers are up and running** before you proceed with testing.
{% endhint %}

{% content-ref url="../installation.md" %}
[installation.md](../installation.md)
{% endcontent-ref %}

## Local API

If you'd like to test the endpoints, you can do this with Postman. Register for and install Postman from their [website](https://www.postman.com). We have a collection of tests already available that you can run. Request access from any of the backend team members to our collections.

Or use curl in your terminal.

{% hint style="success" %}
Use [http://localhost:5000/](http://localhost:5000/) in Postman or curl to make a request to your local API container
{% endhint %}

## Local WEB App

Your local `climatemind-backend_webapp` container allows you to test web-application directly in your browser.&#x20;

{% hint style="success" %}
Go to [http://localhost:3000/](http://localhost:3000/) to see your local web app instance.
{% endhint %}

## Send Sendgrid emails from local 

To be able to send emails from local machine you have to set two environment variables `SENDGRID_API_KEY` and `MAIL_DEFAULT_SENDER`.
See how to set them [here](work-with-docker.md#use-environment-variables).
If you see `python_http_client.exceptions.BadRequestsError: HTTP Error 400: Bad Request` error check the `e.to_dict` which contain response from SendGrid. 
