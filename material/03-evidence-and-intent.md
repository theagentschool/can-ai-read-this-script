# Evidence is not intent

An observed operation supports a claim about behavior. It does not, by itself, prove
why an author included it. Likewise, an AI refusal is evidence about that interaction,
not proof that the code is harmful or that its author planted a trap.

When reporting a finding, attribute claims to their source and distinguish:

- **Observed in the artifact:** names, guards, calls, and the data they address.
- **Reported by a researcher:** what they say happened when they tried particular
  models and prompts.
- **Interpretation:** a possible explanation, such as deliberate anti-LLM obfuscation.
- **Unverified:** whether the conditional path executed, whether a download succeeded,
  or what the author intended, unless the source provides evidence.

The [veritas article](https://nullpt.rs/fingerprinting-bioweapons) reports Astra and
GLM-5.3 outcomes and argues that the decoys may target model safeguards. Attribute
those results to the author; do not present this course as an independent reproduction.
