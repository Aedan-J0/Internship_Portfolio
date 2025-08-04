# Fixing the encoder_attention_mask Warning
## The Problem
I encountered this warning when trying to encode the dictionarys Key: Value pairs and running code with a BERT model:
```console
FutureWarning: encoder_attention_mask is deprecated and will be removed in version 4.55.0 for BertSdpaSelfAttention.forward.
```
Initially, I suspected an issue with my code, but I wasn't using encoder_attention_mask anywhere explicitly. The root cause turned out to be the tokenizer's behavior when processing two separate inputs:
```console
pythontokenizer(user_query, chatgpt_response, ...)
```
This pattern triggers the warning because the model no longer expects the encoder_attention_mask argument.

# The Solution
Instead of passing two separate strings to the tokenizer, I combined them into a single input:
```console
pythoncombined_input = user_query + " " + chatgpt_response
encoded = tokenizer(
    combined_input,
    return_tensors='pt',
    padding=True,
    truncation=True
)
```
This approach ensures the tokenizer only generates the standard attention_mask, eliminating the deprecation warning.

# Result
The warning no longer appears, and the code functions correctly. No modifications to library files or complex workarounds were necessary — simply providing one string instead of two resolved the issue.
