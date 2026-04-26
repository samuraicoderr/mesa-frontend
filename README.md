# MESA — Medical Expert System Assistant

![MESA Demo Screenshot](/sen-grp-1-frontend.vercel.app_mesa.png)

MESA (Medical Expert System Assistant) is a hybrid medical support system that combines a language model with a rule-based expert system. The goal is simple: let users describe how they feel in plain English, then turn that into possible conditions using structured reasoning.

It is built with a Next.js frontend and a Django Ninja backend.

---

## What it does

MESA takes a conversational input from a user, pulls out relevant symptoms, runs them through an inference engine, and returns possible conditions along with a clear explanation.

---

## How it works

1. The user describes symptoms in natural language
2. A language model (like LLaMA) extracts key symptoms from the text
3. Those symptoms are passed into an Experta-based inference engine
4. The engine evaluates predefined medical rules
5. Possible conditions are returned
6. The AI layer adds a readable explanation for the user

The idea is to combine the flexibility of AI with the structure of an expert system.

---

## Tech stack

Frontend

* Next.js

Backend

* Django Ninja
* Experta (rule engine)

AI layer

* LLaMA (or similar LLMs)

---

## Why this approach

Pure LLM systems can sound convincing but are not always consistent. Rule-based systems are consistent but rigid.

MESA sits in the middle:

* The LLM understands messy human input
* The rule engine handles actual reasoning

That separation makes the system easier to trust and debug.

---

## Disclaimer

This is not a medical tool and should not be used for diagnosis or treatment.

It is a research/academic project.

---

## Future work

* Better symptom extraction accuracy
* Expanded medical rule base
* Confidence scoring for outputs
* Improved UI/UX
* Support for more languages

---

## Authors

Built as part of a final year project.
