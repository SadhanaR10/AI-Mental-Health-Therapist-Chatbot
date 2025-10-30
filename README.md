# AI-Mental-Health-Therapist-Chatbot
An AI-powered virtual mental health support system developed using the RASA framework that provides personalized therapy through chatbot interactions. It leverages NLP and machine learning to understand user emotions, offer tailored guidance, and recommend professionals.The system achieved 100% accuracy in conversation and action-level evaluations.

**Key Technologies Used**

Programming Language: Python 3.10

Framework: RASA 3.0

Frontend: React JS with Tailwind CSS

Backend: Python (RASA action server)

Tools: IntelliJ IDEA, Pandas, Materialize CSS

OS: Windows 10

Datasets: Kaggle and Reddit

**Workflow**

1.User Interaction:
The user accesses the web-based chatbot interface (built with React JS and Tailwind CSS) and starts a conversation by selecting their category — Student, Employee, or Non-Employee.

2.Message Processing (Frontend to Backend):
The user’s input is sent to the RASA backend through a REST API webhook, where the message is analyzed for intent and entities using the Natural Language Understanding (NLU) module.

3.Intent & Entity Recognition:
The DIET Classifier and Featurizers identify what the user wants (intent) and extract details (entities) such as “language preference” or “issue type” (e.g., stress, exam pressure).

4.Dialogue Management:
Based on the conversation context, RASA Core uses TEDPolicy, RulePolicy, and MemoizationPolicy to predict the next appropriate action — for example, providing advice, asking a follow-up question, or recommending a doctor.

5.Action Execution:
If the chatbot needs to fetch information (like recommending a doctor), it triggers a custom action from the action server, which processes data from the “doctor_appointment.xlsx” file to find the best match.

6.Response Generation:
The selected action generates a text response, which RASA sends back to the frontend, where it appears in the chat interface as an empathetic message or recommendation.

Continuous Learning & Feedback:
The chatbot’s performance is monitored using conversation and action-level evaluations to refine future responses and maintain 100% accuracy.
