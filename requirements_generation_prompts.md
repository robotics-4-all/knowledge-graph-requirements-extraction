# Requirements Generation Prompts

## Enhanced MCP Prompt (KG-Grounded Approach)

Give me 15 functional requirements for the Deep Learning domain, so that, 
based on these, I will create the syntax of a domain-specific language that 
enables citizen developers to easily configure and set up Deep Learning 
pipelines without deep technical knowledge of the domain.
If you want to use more than one tool, do so without asking for permission. 
You have exactly ONE tool-use round.
Your goal is to identify Functional Requirements (FRs) for a Domain-Specific 
Language (DSL) for the Deep Learning domain.
The FRs must focus on dataset definition, multi-stage training workflows, 
transfer learning—including pretrained or checkpoint initialization, freezing 
and unfreezing, and head replacement—and retraining triggers or strategies 
involving new data, metric degradation, or drift.
The FRs MUST belong ONLY to the provided domain and NOT to related domains.
If the domain name is complex—for example, Robot Operating System—split it 
into its component words, such as robot, operating, and system. Run the 
necessary tools using:
(a) the domain abbreviation, such as ros;
(b) each component word as a separate argument; and
(c) the stem of every word in the domain name, using the NLTK Snowball stemmer.
All tool arguments MUST be lowercase.
For every Functional Requirement produced, clearly mention ALL the 
relationships from which it was derived.
Assume the user has basic familiarity with the domain but no deep technical 
knowledge.
Each FR MUST be phrased as a capability of the DSL—for example, 
"The grammar should support: …"—and must describe what the DSL should 
express, parameterize, or validate, NOT how it should be implemented.
Do NOT reference algorithms, libraries, or framework implementations in 
the FRs. The DSL must remain usable by non-experts. Do not use the words 
"algorithms," "libraries," or "frameworks."
At the end of your response, list all tools used together with the exact 
arguments passed to each.

## Standalone LLM Prompt (No KG Access)

Give me 15 functional requirements for the Deep Learning domain, so that, 
based on these, I will create the syntax of a domain-specific language that 
enables citizen developers to easily configure and set up Deep Learning 
pipelines without deep technical knowledge of the domain.
Your goal is to identify Functional Requirements (FRs) for a Domain-Specific 
Language (DSL) for the Deep Learning domain.
The FRs must focus on dataset definition, multi-stage training workflows, 
transfer learning—including pretrained or checkpoint initialization, freezing 
and unfreezing, and head replacement—and retraining triggers or strategies 
involving new data, metric degradation, or drift.
The FRs MUST belong ONLY to the provided domain and NOT to related domains.
Assume the user has basic familiarity with the domain but no deep technical 
knowledge.
Each FR MUST be phrased as a capability of the DSL—for example, 
"The grammar should support: …"—and must describe what the DSL should 
express, parameterize, or validate, NOT how it should be implemented.
Do NOT reference algorithms, libraries, or framework implementations in 
the FRs. The DSL must remain usable by non-experts. Do not use the words 
"algorithms," "libraries," or "frameworks."

## Note

The same prompt structure was used for all three DSLs (Deep Learning, 
Machine Learning over Data Streams, NLP Pipelines and Machine Learning), 
with the domain name and domain-specific focus areas adapted accordingly 
for each DSL. The only difference between the Enhanced MCP and Standalone 
LLM approaches was whether the MCP tools providing access to the Knowledge 
Graph were available to the model during generation.