<!-- Start SDK Example Usage [usage] -->
### Get Markdown from a URL (GET)

Directly return page markdown content from the request URL.

```typescript
import { DeepcrawlApp } from "@deepcrawl-sdk/ts";

const deepcrawlApp = new DeepcrawlApp({
  bearer: "Bearer <YOUR_API_KEY_HERE>",
});

async function run() {
  const result = await deepcrawlApp.getMarkdown({
    url: "example.com",
  });

  console.log(result);
}

run();

```

### Read URL (POST)

Returning full result object from the request URL.

```typescript
import { DeepcrawlApp } from "@deepcrawl-sdk/ts";

const deepcrawlApp = new DeepcrawlApp({
  bearer: "Bearer <YOUR_API_KEY_HERE>",
});

async function run() {
  const result = await deepcrawlApp.readUrl({
    url: "https://example.com",
  });

  console.log(result);
}

run();

```

### Extract Links from a URL (POST)

Returning extracted links sitemap results for the request URL.

```typescript
import { DeepcrawlApp } from "@deepcrawl-sdk/ts";

const deepcrawlApp = new DeepcrawlApp({
  bearer: "Bearer <YOUR_API_KEY_HERE>",
});

async function run() {
  const result = await deepcrawlApp.extractLinks({
    url: "https://example.com",
  });

  console.log(result);
}

run();

```
<!-- End SDK Example Usage [usage] -->