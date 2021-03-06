---
layout: post
title: New Terms and Conditions
date: 2015-12-15 17:55
author: anya.stettler
comments: true
categories: [older]
product: avaTax
doctype: blog
redirect_to: https://www.avalara.com/us/en/blog/2015/12/new-terms-conditions.html
---
Avalara just posted a new version of our <a href="http://www.avalara.com/new-terms/">AvaTax terms and conditions</a>, effective January 1, 2016. New Ts and Cs are always an opportunity for some fun recreational reading, but these are especially exciting. From section 3.b.ii:
<blockquote> ii. If Customer does submit Documents to the AvaTax Service in a billing month, but usage of the AvaTax APIs or the number of invoice lines submitted significantly exceeds ordinary AvaTax usage in that month, the following calculations may be used to determine “Document” usage during that month:
1. Every 50 API calls to the address validation service will count as one “Document”;
2. Every 100 API calls to the tax calculation service will count as one “Document”; and
3. Every 1,000 invoice lines sent to the tax calculation service will count as one “Document”.</blockquote>
That's a big change! Our existing terms of service only allow 10 address validation calls, 10 tax calculations, or 35 line items before that count outbilled your finalized transactions!

Unnecessary API calls should still be avoided (100 is still finite, and no need to introduce additional processing time where it isn't needed), but this ratio should allow integrations a little more flexibility.

Another big change can be found in section 3.a:
<blockquote>All such records will be considered Documents, regardless of the tax result generated by the AvaTax Service, except for records on which no tax is calculated solely because the Customer has configured the AvaTax Service to not calculate tax on transactions in the jurisdiction of the destination address included on the record.</blockquote>
Prior to January 1, 2016, we counted calculations and documents as billable regardless of their destination or the tax calculated on them. After the change, we will not bill for non-nexus transactions (that is, transactions with ship-to addresses in non-nexus states). This will have the biggest impact on businesses with limited state registrations, and removes the need to "suppress" non-nexus calls to the AvaTax service.

I'm just highlighting some interesting changes here - there are still caveats and exceptions in the new terms that you should be aware of - but this does represent a significant change from our current 2015 terms. Happy reading!
