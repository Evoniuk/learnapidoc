{: .activity_subtitle}
## <i class="fa fa-user-circle"></i> Activity: Evaluate API reference docs for core elements
{% if page.permalink == "/workshop.html" %}{:.no_toc}{% endif %}

In this activity, you'll review API reference documentation and identify the common elements. To evaluate the API reference docs:

1.  Choose three of the following sites. In the three you choose, analyze the API reference sections (where the endpoints are listed):

    *  [Nexmo API reference](https://developer.nexmo.com/api)
    *  [Twitter API reference](https://developer.twitter.com/en/docs/api-reference-index)
    *  [Stripe API reference](https://stripe.com/docs/api)
    *  [Azure API reference](https://docs.microsoft.com/en-us/rest/api/advisor/)
    *  [Flickr API reference](https://www.flickr.com/services/api/)
    *  [YouTube API reference](https://developers.google.com/youtube/v3/docs)
    *  [Splunk API reference](https://docs.splunk.com/Documentation/Splunk/8.0.0/RESTREF/RESTlist)
    *  [Paypal API reference](https://developer.paypal.com/docs/api/overview/)
    *  [Basecamp API reference](https://github.com/basecamp/bc3-api)
    *  [OpenSecrets API reference](http://www.opensecrets.org/open-data/api-documentation)
    *  [Dropbox API reference](https://www.dropbox.com/developers/documentation/http/documentation)
    *  [DBS Developers API](https://www.dbs.com/dbsdevelopers/discover/deposit.html)
    *  [Adyen Docs](https://docs.adyen.com/)
    *  [NBG Technology Hub](https://developer.nbg.gr/apiProducts)

2.  In the reference documentation, identify each of the following sections (if they exist):

    *  [Resource description]({{site.rooturl}}docapis_resource_descriptions.html)
    *  [Endpoints and methods]({{site.rooturl}}docapis_resource_endpoints.html)
    *  [Parameters]({{site.rooturl}}docapis_doc_parameters.html)
    *  [Request example]({{site.rooturl}}docapis_doc_sample_requests.html)
    *  [Response example and schema]({{site.rooturl}}docapis_doc_sample_responses_and_schema.html)

    {: .note}
    The sections might be named differently in the API doc sites you browse, but they're usually recognizable to some degree (if included). If you're finding it somewhat difficult to locate them, this is part of the wild west of terminology and organization when it comes to API documentation.

3.  Assess the API reference documentation by answering the following questions for each section:

    **Resource description:**
      *  Is the description action-oriented?
      *  Is it a brief 1-3 sentence summary?

    **Endpoints and methods:**
      *  How are the endpoints grouped? (Are they listed all on the same page, or on different pages? Are they grouped by method, or by resource?)
      *  How are the methods specified for each endpoint?

    **Parameters:**
      *  How many types of parameters are there (header, path, query string) or request body for the endpoints?
      *  Are the data types (string, boolean, etc.) defined for each parameter? Are required/optional values noted?

    **Request example:**
      *  In what format or language is the request shown (e.g. curl, specific languages, other)?
      *  How many parameters does the sample request include?

    **Response example:**
      *  Is there both a sample response *and* a response schema? (And is each element in the response actually described?)
      *  How does the doc site handle nested hierarchies in the response definitions?

{% if page.workshop_activities == true %}*For more information related to this activity, see [Evaluate API reference docs for core elements]({{site.rooturl}}docapis_api_reference_activity.html).*{% endif %}
