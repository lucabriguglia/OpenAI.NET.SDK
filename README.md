# OpenAI.NET _(Preview)_
.NET SDK for OpenAI with a Blazor Server playground _(available soon)_

[![Main](https://github.com/lucabriguglia/OpenAI.NET/actions/workflows/main.yml/badge.svg)](https://github.com/lucabriguglia/OpenAI.NET/actions/workflows/main.yml)
[![Nuget Package](https://img.shields.io/badge/nuget-1.0.0-blue.svg)](https://www.nuget.org/packages/OpenAI.NET.SDK)

```
Install-Package OpenAI.NET.SDK
```

## APIs

- Models
- Completions
- Edits
- Images
- Embeddings
- Files
- Fine-tunes _(available soon)_
- Moderations _(available soon)_

## Configuration

### Option 1

```C#
services.AddOpenAIClient();
```

This option requires an appsettings.json file

```json
{
  "OpenAI": {
    "ApiKey": "YOUR_API_KEY",
    "Organization": "OUR_ORGANIZATION"
  }
}
```

### Option 2

```C#
services.AddOpenAIClient(options =>
{
     options.ApiKey = "YOUR_API_KEY";
     options.Organization = "YOUR_ORGANIZATION";
 });
```

## Usage

Inject `IOpenAIClient` interface into your service

_(complete guide available soon)_
