# REFLECTION: InventoryHub Development with Microsoft Copilot

**Author:** Lawrence Babelonia

## Activity 1: Generating Integration Code
Copilot helped me scaffold the initial communication between the Blazor front-end and .NET back-end. It suggested how to use `HttpClient`, model the `Product` and `Category` classes, and create a simple fetch method.

## Activity 2: Debugging and Fixing Issues
When I encountered CORS issues and mismatched routes, Copilot recommended the correct use of `app.UseCors()` and `Http.GetAsync()` adjustments. It also suggested using `try-catch` for handling malformed JSON responses.

## Activity 3: Structuring JSON Responses
I used Copilot to create a clean, nested JSON format with a `Category` object inside each `Product`. It ensured naming conventions matched C# models and improved consistency between front-end and back-end.

## Activity 4: Optimizing for Performance
Copilot guided me to implement `IMemoryCache` on the back-end to reduce repeated computation and data fetches. It also suggested avoiding redundant API calls in Blazor components by tracking state.

## What I Learned
I learned to work more efficiently with AI support. Copilot is most helpful when:
- I write clear method summaries as comments.
- I need fast, boilerplate generation.
- I want ideas for best practices or optimization.

Copilot didn’t replace my reasoning, but it made me faster, cleaner, and more consistent in my full-stack development process.