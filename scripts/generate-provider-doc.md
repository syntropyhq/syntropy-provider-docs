# How to Generate Provider Documentation

## Process

1. **Research the Provider**
   - Visit their main website and documentation
   - Review their pricing page
   - Read their API documentation
   - Check their GitHub repos (if applicable)

2. **Use an LLM to Generate the Summary**

   Use this prompt with Claude/GPT:

   ```
   I need you to create a structured documentation summary for [PROVIDER_NAME].

   Visit their website at [WEBSITE_URL] and review their documentation.

   Generate a markdown document with the following sections:

   # [Provider Name]

   ## Overview
   [2-3 sentences explaining what the provider does and their core value proposition]

   ## Key Features
   [Bulleted list of main capabilities and offerings]

   ## Use Cases
   [Common scenarios where this provider is used]

   ## Pricing
   [Pricing model overview - free tier, paid tiers, pricing structure]

   ## Integration
   [How developers integrate - APIs, SDKs, supported languages/frameworks]

   ## Comparison Points
   [Key differentiators vs alternatives - what makes them unique or different]

   ## Support & Resources
   [Links to docs, community, support channels, status pages]

   Keep it concise but informative. Focus on information that would help someone understand if this provider fits their needs and how it compares to alternatives.
   ```

3. **Review and Edit**
   - Verify accuracy of pricing and features
   - Ensure comparison points are fair
   - Check that links are correct

4. **Save to Repository**
   - Filename: `providers/{provider-slug}.md` (lowercase, hyphens for spaces)
   - Commit with message: `Add {Provider Name} documentation`
   - Push to main branch

5. **Update Syntropy Broker**
   - Add entry to PROVIDER_FIXTURES in the main Syntropy repo
   - Use the raw GitHub URL for readmeUrl

## File Naming Convention

- Use lowercase
- Use hyphens for multi-word names
- Examples:
  - `stripe.md`
  - `vercel.md`
  - `aws-s3.md`
  - `google-cloud-run.md`

## Quality Checklist

- [ ] All sections present and filled out
- [ ] Pricing is current and accurate
- [ ] Links work and go to official resources
- [ ] Comparison points are fair and factual
- [ ] Use cases are specific and realistic
- [ ] Integration details are technically accurate
