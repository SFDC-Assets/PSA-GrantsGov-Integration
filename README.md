![Public Sector Accelerators logo](/docs/Logo_GPSAccelerators_v01.png)

# Grants.gov Integration

Interact with Grants.gov APIs with this MuleSoft Connector.

Accelerator Listing: [insert url to the public listing on the Accelerator site](https://pubsec-accelerators.my.site.com/accelerators/) (tbd once published)


## Description

[Required. Description of the Accelerator. This should match the approved content used on the Accelerator listing, but could include additional content. This can include images/screenshots which must be stored in the /docs/ folder (no external images or images stored elsewhere in the repository.]

As Grants.gov remains a place for where grant opportunities are published for wider socialization by grantors and a platform for applicants to acquire necessary information, apply for the grants and supply the updates on their projects, it is imperative that any Grants Management system has a meaningful integration with Grants.gov. 

With Salesforce Grants Management Application, a grantor can see all grant recipients, gain insights into spending and view specific milestones. Meanwhile, the grantee can view the grant programs they’re enrolled in ,implementation and milestone status, compliance records and more. These capabilities can be extended and augmented with a deeper integration with the Grants.gov, Pay.gov and SAM.gov system to system interfaces. 

This is where MuleSoft comes in the picture. MuleSoft Anypoint Platform comes with a set of prescriptive blueprints to build API driven Integrations and a library of Pre-Built components that enable organizations to extend and enrich Salesforce Grants Program Management Application. This white paper will provide technical details on how these integrations can be implemented and how MuleSoft can provide necessary acceleration while enhancing Salesforce Grants Management Application to deliver a highly differentiated solution while increasing the returns of investments for the Salesforce customer base. 


## Included Assets

[Required. List of the assets included in the Accelerator and where to find them. This can be as detailed as desired, but at a minimum it should be detailed by asset type (unmanaged package, datapack, documentation, and other assets) and the next level metadata type (Salesforce metadata, datapack contents, separate documentation files, etc.) and their counts.]

This Accelerator includes the following assets:
<ol>
 <strong> Under Specifications Folder: </strong>
 <ul> <li>  API Specifications in RAML to build a System API for Grants.gov Applicant System to Syetem Interface.  that includes  </li>
  <li>API Specifications in OAS to build a System API for Grants.gov Applicant System to Syetem Interface.</li></ul>
  <strong>Under Implementation Folder: </strong>
  <ul><li> Fully functional Example Mule System API for Grants.gov Applicant System to Syetem Interface  which can be imported into MuleSoft AnyPoint Studio 7.15 and above. </li>
    </ul>
   <strong>Documentation</strong>, including:
    <ul>
      <li>This readme file</li>
      <li>White paper providing detailed setup instructions and a data dictionary (located in the /docs/ folder)</li>
    </ul>
</ol>


## Before You Install

[Required. Pre-requisites, dependencies, license requirements, and other assumptions and caveats should be declared here. Consider content that's specific to the Accelerator and the type of product or technology involved. The PMO may also add assumptions or notes that more broadly apply to the entire program.]

**Setting up System To System with Grants.gov**
1) This section assumes that your organization is already set up with EBiz POC account on the Grants.gov User Interface.
2) For clients connecting to Grants.gov Web Services for the first time:
- Obtain a digital certificate and ensure it is properly set up to communicate securely via a mutual authentication with Grants.gov. See the Applicant Certificates.
- Grants.gov S2S interfaces require authentication of the end user’s identity through a personal user authentication certificate that utilizes a 2048 bit public RSA key and a SHA-2 based digital signature. A personal user authentication certificate is also known as an SSL client, PKI, web browser, or email certificate and must be purchased from a recognized Certificate Authority (CA). Grants.gov S2S team provides a PDF form that can be used to submit the user authentication certificate to be loaded on the server side. 
- Become familiar with the Grants.gov Hashing Standards.

If you have questions regarding gaining access to the Grants.gov S2S interface, please contact Grants.gov.


**License Requirements** [Required]
* Example: License Public Sector Solutions - requires Foundations or Advanced for internal; requires Communities for external

**Accelerator or Technology-Specific Assumptions** [Optional]
* Example: You have installed and configured OmniStudio and provided permission to PSS objects.
* Example: You are using OmniStudio's native runtime.

**General Assumptions** [Optional]
* Example: You are using this Accelerator in a sandbox or test environment. It is recommended that you not install any Accelerator directly into production environments.)
* Example: If you do not have a Salesforce org licensed to you, you may try Public Sector Solutions for free with one of our [trial environments](https://developer.salesforce.com/free-trials/comparison/public-sector).
* Example: You are using this Accelerator in conjunction with the Salesforce Lightning Experience (LEX) - not the Classic UI.


## Installation

[Required. Steps necessary for installing the Accelerator. This can include images/screenshots which must be stored in the /docs/ folder (no external images or images stored elsewhere in the repository.]

**Grants.gov Applicant S2S - System API Implementation**
This project contains a pre-built API implementation that you can customize. This implementation provides an APIKit enabled System API which showcases how to surface the Applicant S2S operations as a RESTful API. This asset can be used with AnyPoint Studio version 7.15+ . 

It showcases examples of the following:
   1) An Extensible, APIKit enabled Mule API built using RAML Specifications for the Grants.gov Applicant S2S System API
   2) Configuration of the Web Services Consumer Connector to demonstrate how Grants.gov S2S interface can be consumed
   3) Preparation of the xml payloads that are required to invoke Grants.gov S2S operations
   4) Transformation of XML outputs from the Grants.gov S2S operations to JSON format

**Importing Example Application into Anypoint Studio**
1) Download the grants-applicant_webservices_system_api-v3.jar file that is attached with this project under Implementation Folder. 
2) Open AnyPoint Studio and Go to File → Import
3) Select Packaged Mule Application option from AnyPoint Studio category
4) Navigate to the location where the jar file was downloaded in the step 1. 
5) Click Finish. 

**Running Templates in Anypoint Studio**
After you import your template into Studio, follow these configuration steps to run it.
1) Right-click the project folder.
2) Hover your mouse over 'Run as'.
3) Click Mule Application (configure).
4) Inside the dialog, select Environment and set the variable mule.env to the appropriate value (e.g., dev or local).
5) Inside the dialog, select Environment and set the variable mule.encryptionKey to the property encryption key that you used to encrypt your secure properties.
6) Inside the dialog, go to 'Clear Application Data' select 'always' radio button.
7) Click Run.
 
** Additional Information**
1) Please refer to the attached link on how to secure the configuration properties.
   https://docs.mulesoft.com/mule-runtime/4.4/secure-configuration-properties
3) Please refer to the attached link on how to generate the Keystore.
   https://docs.mulesoft.com/mule-runtime/4.4/tls-configuration
5) This solution was developed and tested on Anypoint Studio 7.15 and Mule Runtime 4.4.0.

## Post-Install Setup & Configuration

[Required. Steps necessary for using the Accelerator. This can include images/screenshots which must be stored in the /docs/ folder (no external images or images stored elsewhere in the repository.]


## FAQs

[Optional. Preemptive list of common questions or situations that need to be explained in how the Accelerator works (or doesn't).]

**_Q: Do I really need an FAQ for my Accelerator?_**

A: Great question! Perhaps not, but if you had common misunderstandings or confusion during beta testing with an aspect of setup or use, you may find it helpful to create some related FAQs. You might also wish to use FAQs to reiterate a critical point found in this readme or any other included documentation. An FAQ may also help point out a recommendation or tip about how to use your Accelerator.

## Additional Resources

[Optional. Summary list of additional links and references that you think are useful to. These links should be restricted to official Salesforce web resources and should not include third party references. Use an unordered list.]


## Revision History

[Required. High level description of the Accelerator's versions, with the date it was made publicly available. If more detailed release notes or change log are necessary, create a separate readme in the same folder and link to it from here.]
<strong>1.0 Initial release (30 Oct 2023)</strong> - Short description of the release. For detailed release notes and change logs, provide a link to another readme in the /docs/ folder of this repository.


## Acknowledgements

Creator:  **[Afzal Memon](https://github.com/az-mulesoft)**, Distinguished Solution Engineer, Salesforce


## Terms of Use

Thank you for using Public Sector Accelerators.  Accelerators are provided by Salesforce.com, Inc., located at 1 Market Street, San Francisco, CA 94105, United States.

By using this site and these accelerators, you are agreeing to these terms. Please read them carefully.

Accelerators are not supported by Salesforce, they are supplied as-is, and are meant to be a starting point for your organization. Salesforce is not liable for the use of accelerators.

For more about the Accelerator program, visit: [https://pubsec-accelerators.my.site.com/accelerators/](https://pubsec-accelerators.my.site.com/accelerators/)
