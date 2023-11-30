![Public Sector Accelerators logo](/docs/Logo_GPSAccelerators_v01.png)

# Grants.gov Integration

Interact with the Grants.gov Applicant API with this MuleSoft Connector.

Accelerator Listing: [insert url to the public listing on the Accelerator site](https://pubsec-accelerators.my.site.com/accelerators/) (tbd once published)


## Description

This Accelerator provides a pre-built integration with Grants.gov's Applicant System to System (S2S) inteface.  This implementation provides an APIKit enabled System API which showcases how to surface the Grants.gov Applicant S2S operations as a RESTful API. This asset can be used with MuleSoft AnyPoint Studio and customized for your own needs.  It showcases examples of the following:
* an extensible, APIKit enabled MuleSoft API built for the Grants.gov Applicant S2S System API using RAML specifications
* configuration of the Web Services Consumer Connector to demonstrate how Grants.gov S2S interface can be consumed
* preparation of the XML payloads that are required to invoke Grants.gov S2S operations
* transformation of XML outputs from the Grants.gov S2S operations to JSON format

As Grants.gov remains a place for where grant opportunities are published for wider socialization by grantors and a platform for applicants to acquire necessary information, apply for the grants and supply the updates on their projects, it is imperative that any grants management system has a meaningful integration with Grants.gov.

With a Salesforce-based grants management app, a grantor can see all grant recipients, gain insights into spending, and view specific milestones. Meanwhile, the grantee can view the grant programs they’re enrolled in, implementation and milestone status, compliance records, and more. These capabilities can be extended and augmented with a deeper integration with the Grants.gov, Pay.gov and SAM.gov system-to-system interfaces. 

This is where MuleSoft comes into the picture.  MuleSoft Anypoint Platform comes with a set of prescriptive blueprints for building API-driven integrations and a library of pre-built components that enable organizations to extend and enrich Salesforce grants management application. This white paper will provide technical details on how these integrations can be implemented and how MuleSoft can provide necessary acceleration while enhancing Salesforce Grants Management Application to deliver a highly differentiated solution while increasing the returns of investments for the Salesforce customer base.


## Included Assets

This Accelerator includes the following assets:
<ol>
 <li><strong>APIs</strong>, including:
  <ul>
   <li>API specifications in RAML and OAS (see the /mulesoft/specifications/ directory)</li>
   <li>Fully functional example MuleSoft System API for Grants.gov (see the /mulesoft/implementation/ directory)</li>
  </ul>
 </li>
 <li><strong>Documentation</strong>, including:
  <ul>
   <li>White paper providing detailed setup instructions and a data dictionary (located in the /docs/ directory)</li>
   <li>This readme file</li>
  </ul>
</ol>


## Before You Install

**Access to Grants.gov**
* This Accelerator assumes that your organization is already authorized and set up to access the Grants.gov Applicant S2S interface (please refer to [Grants.gov documentation](https://www.grants.gov/system-to-system/applicant-system-to-system/)).

**License Requirements**
* This solution was developed and tested on Anypoint Studio v7.15 and Mule Runtime v4.4.0; you should be running these or higher versions.
* ANY OTHER SALESFORCE LICENSE REQUIREMENT? (example: Requires Public Sector Solutions)

**Other Assumptions**
* WHAT VERSION OF THE GRANTS.GOV API DOES THIS COMPLY WITH?
* You are using this Accelerator in a sandbox or test environment. It is recommended that you not install any Accelerator directly into production environments without proper testing.


## Installation

Please refer to the white paper (see /docs/ directory) for detailed installation instructions.

To import the example application into MuleSoft AnyPoint Studio:
1) Download the grants-applicant_webservices_system_api-v3.jar file (see the /mulesoft/implementation/ directory).
2) Open AnyPoint Studio and go to File → Import.
3) Select the Packaged Mule Application option from AnyPoint Studio category.
4) Navigate to the location where the jar file was downloaded.
5) Click Finish.


## Post-Install Setup & Configuration

Please refer to the white paper (see /docs/ directory) for detailed configuration instructions and documentation.

To run a template after you import it into AnyPoint Studio, follow these configuration steps:
1) Right-click the project folder.
2) Hover your mouse over 'Run as'.
3) Click Mule Application (configure).
4) Inside the dialog, select Environment and set the variable mule.env to the appropriate value (e.g., dev or local).
5) Inside the dialog, select Environment and set the variable mule.encryptionKey to the property encryption key that you used to encrypt your secure properties.
6) Inside the dialog, go to 'Clear Application Data' select 'always' radio button.
7) Click Run.


## FAQs

**_Q: How do I get support for accessing and configuring Grants.gov APIs and services?_**

A: For all Grants.gov questions, troubleshooting, and support, you must contact Grants.gov directly and refer to their documentation.


## Additional Resources

* [Secure Configuration Properties](https://docs.mulesoft.com/mule-runtime/4.4/secure-configuration-properties)
* [Configure TLS with Keystores and Truststores](https://docs.mulesoft.com/mule-runtime/4.4/tls-configuration)


## Revision History

**v1.0 (20 Nov 2023)** - Initial release of the Accelerator.


## Acknowledgements

Creator:  **[Afzal Memon](https://github.com/az-mulesoft)**, Distinguished Solution Engineer, Salesforce


## Terms of Use

Thank you for using Public Sector Accelerators.  Accelerators are provided by Salesforce.com, Inc., located at 1 Market Street, San Francisco, CA 94105, United States.

By using this site and these accelerators, you are agreeing to these terms. Please read them carefully.

Accelerators are not supported by Salesforce, they are supplied as-is, and are meant to be a starting point for your organization. Salesforce is not liable for the use of accelerators.

For more about the Accelerator program, visit: [https://pubsec-accelerators.my.site.com/accelerators/](https://pubsec-accelerators.my.site.com/accelerators/)
