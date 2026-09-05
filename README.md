# BankEase AI 🤖🏦

## AI-Powered Banking Customer Support Chatbot

BankEase AI is an AI-powered banking customer-support chatbot developed using IBM watsonx Assistant. The project is designed to understand common banking customer enquiries, identify the user's intent, extract relevant information, and provide appropriate responses through conversational dialogue.

The project demonstrates how conversational AI can automate routine banking support and provide fast, consistent first-line assistance.

## 🎯 Project Objectives

- Identify common banking customer-service enquiries
- Create and train banking-related intents
- Define entities to extract relevant information
- Design structured dialog conversation flows
- Implement child nodes for multi-step conversations
- Use options and follow-up questions
- Test the chatbot using different customer scenarios
- Evaluate expected and actual responses
- Identify limitations and possible improvements

## 🧠 AI Components

BankEase AI uses the following components of IBM watsonx Assistant:

- **Intents** – Identify what the customer wants to accomplish
- **Entities** – Extract specific information from customer messages
- **Dialog Nodes** – Control the main conversation flow
- **Child Nodes** – Handle follow-up questions and branching
- **Context Variables** – Preserve information across conversation turns
- **System Entities** – Recognize values such as numbers
- **Options** – Provide predefined choices to customers
- **Wait for Reply** – Enable multi-turn conversations
- **Anything Else** – Handle fallback and unexpected inputs

## 💳 Banking Intents

The chatbot currently supports 13 banking-related intents:

1. Activate Card
2. Cancel Card
3. Fee Inquiry
4. Replace Card
5. Report Missing Card
6. Request Card Member Agreement
7. Request Checkbook
8. Request Increase in Credit Line
9. Set Up Direct Deposit
10. Transfer Money
11. View Account Activity
12. View Pending Charges
13. View Routing Number

## 🏷️ Entities

The chatbot uses custom and system entities such as:

- `@card_type`
- `@card_status`
- `@fee_type`
- `@agreement_type`
- `@checkbook_request_type`
- `@transfer_type`
- `@account_type`
- `@sys-number`

### Example

Customer message:

> "I want to make an international transfer of 5000."

The chatbot identifies:

```text
Intent:
#Banking_Transfer_Money

Entity:
@transfer_type = International Transfer

System Entity:
@sys-number = 5000
