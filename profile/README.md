<h1 align="center">☁️ GroupDocs.Conversion Cloud</h1>

<h3 align="center">Powerful Document Conversion Cloud API for 80+ File Formats</h3>

<p align="center">
  <strong>GroupDocs.Conversion Cloud</strong> is an enterprise-grade REST API for high-fidelity document conversion. Integrate 80+ file format conversions into web, mobile, or desktop applications with no third-party software. Convert PDF, Microsoft Office (Word, Excel, PowerPoint), images, CAD, HTML, and more with full control over the output.
</p>

[![Product Page](https://img.shields.io/badge/Product%20Page-2865E0?style=for-the-badge&logo=appveyor&logoColor=white)](https://products.groupdocs.cloud/conversion/)
[![Docs](https://img.shields.io/badge/Docs-2865E0?style=for-the-badge&logo=Hugo&logoColor=white)](https://docs.groupdocs.cloud/conversion)
[![Demos](https://img.shields.io/badge/Demos-2865E0?style=for-the-badge&logo=appveyor&logoColor=white)](https://products.groupdocs.app/conversion/family)
[![API](https://img.shields.io/badge/API-2865E0?style=for-the-badge&logo=html5&logoColor=white)](https://reference.groupdocs.cloud/conversion/)
[![Blog](https://img.shields.io/badge/Blog-2865E0?style=for-the-badge&logo=WordPress&logoColor=white)](https://blog.groupdocs.cloud/categories/groupdocs.conversion-cloud-product-family)
[![Search](https://img.shields.io/badge/Search-2865E0?style=for-the-badge&logo=searchengin&logoColor=white)](https://search.groupdocs.cloud/)
[![Support](https://img.shields.io/badge/Support-2865E0?style=for-the-badge&logo=Discourse&logoColor=white)](https://forum.groupdocs.cloud/c/conversion/11)
[![Temp License](https://img.shields.io/badge/Temp%20License-2865E0?style=for-the-badge&logo=rocket&logoColor=white)](https://purchase.groupdocs.cloud/cloud/trial/)

---

## Latest Conversion News & Updates

* New Salesforce Free Component [Converter PDF](https://appexchange.salesforce.com/appxListingDetail?listingId=a01f33f8-8539-465d-be77-7067b5e6364a) was deployed. Download and use within the Salesforce APEX SDK
* Published [GroupDocs.Conversion 25.12](https://www.nuget.org/packages/GroupDocs.Conversion/) on NuGet and Maven — performance improvements for PDF/Office to PDF, better font fallback, and leaner HTML output.
* New guides were published at [GroupDocs.Conversion Cloud Blog](https://blog.groupdocs.cloud/categories/groupdocs.conversion-cloud-product-family/).

---

## 📂 Cloud SDKs & Repositories

SDKs are grouped by platform. Each example converts a Word document to PDF using the [Convert document](https://docs.groupdocs.cloud/conversion/convert-document/) API.

### 🌐 .NET (C#, ASP.NET)

.NET SDK for GroupDocs.Conversion Cloud — .NET Core and .NET Framework.

* **[groupdocs-conversion-cloud-dotnet](https://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-dotnet)** — SDK  
* **[groupdocs-conversion-cloud-dotnet-samples](https://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-dotnet-samples)** — Examples

```csharp
var configuration = new Configuration(MyClientId, MyClientSecret);
var apiInstance = new ConvertApi(configuration);
var settings = new ConvertSettings
{
    FilePath = "WordProcessing/four-pages.docx",
    Format = "pdf",
    OutputPath = "converted"
};
var response = apiInstance.ConvertDocument(new ConvertDocumentRequest(settings));
```

### ☕ Java

Java SDK for the GroupDocs.Conversion Cloud REST API.

* **[groupdocs-conversion-cloud-java](https://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-java)** — SDK  
* **[groupdocs-conversion-cloud-java-samples](https://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-java-samples)** — Examples

```java
Configuration configuration = new Configuration(MyClientId, MyClientSecret);
ConvertApi apiInstance = new ConvertApi(configuration);
ConvertSettings settings = new ConvertSettings();
settings.setFilePath("WordProcessing/four-pages.docx");
settings.setFormat("pdf");
settings.setOutputPath("converted");
List<StoredConvertedResult> result = apiInstance.convertDocument(new ConvertDocumentRequest(settings));
```

### 🐘 PHP

PHP SDK for the GroupDocs.Conversion Cloud REST API.

* **[groupdocs-conversion-cloud-php](https://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-php)** — SDK  
* **[groupdocs-conversion-cloud-php-samples](https://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-php-samples)** — Examples

```php
use GroupDocs\Conversion\Model;
use GroupDocs\Conversion\Model\Requests;

$configuration = new GroupDocs\Conversion\Configuration();
$configuration->setAppSid($ClientId);
$configuration->setAppKey($ClientSecret);
$apiInstance = new GroupDocs\Conversion\ConvertApi($configuration);

$settings = new Model\ConvertSettings();
$settings->setFilePath("WordProcessing/four-pages.docx");
$settings->setFormat("pdf");
$settings->setOutputPath("converted");

$result = $apiInstance->convertDocument(new Requests\ConvertDocumentRequest($settings));
```

### 📦 Node.js (JavaScript / TypeScript)

Node.js SDK for the GroupDocs.Conversion Cloud REST API.

* **[groupdocs-conversion-cloud-node](https://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-node)** — SDK  
* **[groupdocs-conversion-cloud-node-samples](https://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-node-samples)** — Examples

```javascript
const conversion_cloud = require("groupdocs-conversion-cloud");
const convertApi = conversion_cloud.ConvertApi.fromKeys(clientId, clientSecret);

let settings = new conversion_cloud.ConvertSettings();
settings.filePath = "WordProcessing/four-pages.docx";
settings.format = "pdf";
settings.outputPath = "converted";

let result = await convertApi.convertDocument(new conversion_cloud.ConvertDocumentRequest(settings));
```

### 🐍 Python

Python SDK for the GroupDocs.Conversion Cloud REST API.

* **[groupdocs-conversion-cloud-python](https://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-python)** — SDK  
* **[groupdocs-conversion-cloud-python-samples](https://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-python-samples)** — Examples

```python
import groupdocs_conversion_cloud

api_instance = groupdocs_conversion_cloud.ConvertApi.from_keys(client_id, client_secret)

settings = groupdocs_conversion_cloud.ConvertSettings()
settings.file_path = "WordProcessing/four-pages.docx"
settings.format = "pdf"
settings.output_path = "converted"

result = api_instance.convert_document(
    groupdocs_conversion_cloud.ConvertDocumentRequest(settings)
)
```

### 💎 Ruby

Ruby SDK for the GroupDocs.Conversion Cloud REST API.

* **[groupdocs-conversion-cloud-ruby](https://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-ruby)** — SDK  
* **[groupdocs-conversion-cloud-ruby-samples](https://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-ruby-samples)** — Examples

```ruby
require 'groupdocs_conversion_cloud'

api_instance = GroupDocsConversionCloud::ConvertApi.from_keys($client_id, $client_secret)

settings = GroupDocsConversionCloud::ConvertSettings.new
settings.file_path = "WordProcessing/four-pages.docx"
settings.format = "pdf"
settings.output_path = "converted"

result = api_instance.convert_document(
  GroupDocsConversionCloud::ConvertDocumentRequest.new(settings)
)
```

### 🔷 Go

Go SDK for the GroupDocs.Conversion Cloud REST API.

* **[groupdocs-conversion-cloud-go](https://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-go)** — SDK  
* **[groupdocs-conversion-cloud-go-samples](https://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-go-samples)** — Examples

```go
settings := models.ConvertSettings{
    FilePath:   "WordProcessing/four-pages.docx",
    Format:     "pdf",
    OutputPath: "converted",
}
result, _, err := config.Client.ConvertApi.ConvertDocument(config.Ctx, settings)
```

### 🔷 Salesforce and Apex SDL

Use GroupDocs.Conversion Cloud from Salesforce via Apex: deploy the Cloud SDK for Apex, then call the Conversion API (upload, convert, download) from your org. The demos below include a free converter component and a sample application.

* **[groupdocs-comparison-cloud-apex](https://github.com/groupdocs-comparison-cloud/groupdocs-comparison-cloud-apex)** — GroupDocs Cloud SDK for Apex (configuration, file storage, and API clients; use with Conversion and other Cloud APIs).
* **[GroupDocs.Salesforce-Demo](https://github.com/groupdocs/GroupDocs.Salesforce-Demo)** — Salesforce demo app with free converter PDF component and document management (preview, compare, convert) using GroupDocs Cloud.
* **[salesforce-conversion-apex-sdk-demo-application](https://github.com/groupdocs-conversion-cloud/salesforce-conversion-apex-sdk-demo-application)** — Sample Salesforce app with Apex SDK examples for GroupDocs.Conversion Cloud.

After deploying the SDK and adding `https://api.groupdocs.cloud` in **Remote Site Settings**, you can convert a document from Apex as follows (upload → convert → optional download). See [GDController.cls](https://github.com/groupdocs/GroupDocs.Salesforce-Demo/blob/main/force-app/main/default/classes/GDController.cls) for a full controller example.

```apex
// Create config and API instances (use your Client Id and Client Secret from https://dashboard.groupdocs.cloud)
Configuration config = new Configuration('YOUR_API_KEY', 'YOUR_API_SECRET');
FileApi fileApi = new FileApi(config);
ConvertApi convertApi = new ConvertApi(config);

// 1. Upload source file to cloud storage
List<ContentVersion> cvList = [SELECT Id, Title, VersionData FROM ContentVersion WHERE Title = 'four-pages.docx' LIMIT 1];
fileApi.uploadFile(new UploadFileRequest('WordProcessing/four-pages.docx', cvList[0].VersionData, null));

// 2. Convert document (e.g. DOCX to PDF)
ConvertSettings settings = new ConvertSettings();
settings.FilePath = 'WordProcessing/four-pages.docx';
settings.Format = 'pdf';
settings.OutputPath = 'converted';

List<StoredConvertedResult> result = convertApi.convertDocument(new ConvertDocumentRequest(settings));
// 3. Download from result[0].Url or use FileApi to get the file
```

---

### Business Use Cases

* **PDF/Office to PDF/A** — Standardize outputs for archiving and e-discovery compliance.
* **PDF archiving** — Convert legacy Office files to PDF/A for long-term storage.
* **Digital previews** — Generate PNG/JPG thumbnails for document portals and mobile apps.
* **CAD exchange** — Convert engineering drawings to PDF for sharing and viewing.
* **Serverless automation** — Use REST calls from AWS Lambda or Azure Functions for on-demand conversion.

---

## 🔑 API Key & Authentication

Use **Client ID** and **Client Secret** from [GroupDocs Cloud Dashboard](https://dashboard.groupdocs.cloud/applications) to authenticate. Set them in your SDK configuration (e.g. `Configuration`, `from_keys`, or environment variables) before calling the API.

---

## ✅ Key Features & Benefits

| Feature | Description |
|--------|-------------|
| **80+ formats** | DOCX, PDF, XLSX, PPTX, HTML, MSG/EML, CAD, Visio, Project, images, and more. |
| **High fidelity** | Preserve layout, fonts, images, vector graphics, and metadata. |
| **Page control** | Convert specific pages, ranges, or consecutive page sets. |
| **Watermarks & protection** | Add text or image watermarks; open and convert password-protected files. |
| **Performance & scale** | Caching, streaming, and linearized PDF output for large documents. |
| **Content options** | Remove annotations/attachments; grayscale or optimize output. |
| **Document info** | Get page count, author, creation date, and other metadata. |

---

## 🆘 Technical Support & Resources

| Resource | Link |
|----------|------|
| **Documentation** | [GroupDocs.Conversion Cloud Docs](https://docs.groupdocs.cloud/conversion/) — guides, API reference, and SDK usage. |
| **Support forum** | [GroupDocs Cloud Free Support Forum](https://forum.groupdocs.cloud/c/conversion/11) — ask questions and report issues. |
| **Temporary license** | [Get a free trial](https://purchase.groupdocs.cloud/cloud/trial/) — full-feature evaluation. |
| **Live demo** | [GroupDocs.Conversion apps](https://products.groupdocs.app/conversion/family) — try conversions in the browser. |
| **API reference** | [REST API Reference](https://reference.groupdocs.cloud/conversion/) — Swagger/OpenAPI. |

---

## 🏷️ Tags

`document-conversion` `file-converter-api` `pdf-to-word` `word-to-pdf` `excel-to-pdf` `ppt-to-pdf` `pdf-to-jpg` `html-to-pdf` `email-to-pdf` `cad-to-pdf` `docx-to-pdf` `pdf-to-docx` `batch-document-conversion` `server-side-conversion` `document-automation` `high-fidelity-conversion` `page-range-conversion` `watermarking-during-conversion` `conversion-sdk`
