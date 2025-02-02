# Bright Data Residential Proxies

[![Promo](https://github.com/luminati-io/Rotating-Residential-Proxies/blob/main/50%25%20off%20promo.png)](https://brightdata.com/proxy-types/residential-proxies) 

## Overview
Experience seamless scraping with Bright Data's [industry-leading residential proxies](https://brightdata.com/proxy-types/residential-proxies), designed to provide precise targeting, unmatched stability, and rapid response times.

- **72M+ Residential IPs**
- **Sticky and rotating sessions**
- **99.95% success rate**
- **HTTP(S) & SOCKS5 support**
- **Geo-location targeting (Free)**

## Key Features
- **Global Coverage**: Residential proxies available in [195 countries](https://brightdata.com/locations).
- **High Success Rates**: Achieve up to 99.95% success in your scraping projects.
- **Fast Response**: Average response time of ~0.7 seconds.
- **Ethically Sourced**: All proxies are sourced with explicit user consent.
- **Unlimited Concurrent Sessions**: Scale your operations without limitations.

## Pricing Plans
- **Pay As You Go**: $8.4/GB, no monthly commitment required.
- **Monthly Subscriptions**:
  - **69 GB**: $7.14/GB, $499/month.
  - **158 GB**: $6.3/GB, $999/month.
  - **339 GB**: $5.88/GB, $1999/month.
  - **Enterprise Plans**: Custom solutions available for large-scale needs.

[![Promo](https://github.com/luminati-io/LinkedIn-Scraper/blob/main/Proxies%20and%20scrapers%20GitHub%20bonus%20banner.png)](https://brightdata.com/proxy-types/residential-proxies) 

## Getting Started with Residential Proxies
1. **Start Free Trial**: No credit card required.
2. **Integration**: Use our APIs or Control Panel to manage IPs and configurations.
3. **Supported Languages**: Quick start examples provided for Python, Java, C#, Node.js, and Shell.

## Code Examples

### Python

```python
import sys

# Replace '[your customerID]', 'residential', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335',
             'https': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335',
             'https': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 33335);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-residential", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:33335");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-residential", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335',
})
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:33335 --proxy-user brd-customer-[your customerID]-zone-residential:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

## Integrations
Our residential proxies integrate with popular tools and frameworks, including:

- [**Puppeteer**](https://brightdata.com/integration/puppeteer)
- [**Selenium**](https://brightdata.com/integration/selenium)
- [**Playwright**](https://brightdata.com/integration/playwright)
- [**AdsPower**](https://brightdata.com/integration/adspower)
- [**MultiLogin**](https://brightdata.com/integration/multilogin)

## Use Cases
Explore how businesses leverage residential proxies:

- [**eCommerce**](https://brightdata.com/use-cases/ecommerce): Track pricing and reviews.
- [**Social Media**](https://brightdata.com/use-cases/social-media-for-marketing): Monitor trends.
- [**Real Estate**](https://brightdata.com/use-cases/real-estate): Gather market data.
- [**Travel**](https://brightdata.com/use-cases/travel): Compare prices across regions.
- [**Financial Services**](https://brightdata.com/use-cases/financial): Analyze trends securely.

## FAQ

### What is a Residential Proxy?
Residential proxies provide IPs from real users, allowing you to gather data as if you’re physically present in specific locations.

### What are the benefits of Residential Proxies?
- Bypass geolocation restrictions
- Conduct web scraping without detection
- Perform market research and price comparison

### What types of plans are available? 
Bright Data offers flexible pricing models, including:

- **Pay-As-You-Go**: Fixed rate per GB.
- **Subscription Plans**: Monthly, yearly, and custom options.

### Are Bright Data's Residential Proxies compliant and safe to use?
Bright Data’s proxies are ethically sourced, and we comply with all relevant data protection laws, including GDPR and CCPA.

### Is there dedicated support available?
Our dedicated support team is available 24/7 to assist you. Contact us to discuss your needs and maximize the benefits of our residential proxy network.
