This project aimed to develop an AI-driven virtual therapist chatbot that provides accessible, personalized, and effective mental health support. The system leverages Natural Language Processing (NLP) and Machine Learning (ML) techniques within the RASA Framework to simulate therapeutic interactions, helping users manage their emotional challenges and connect with mental health professionals when needed.

The project addresses the global shortage of mental health services by offering an intelligent, empathetic, and scalable digital solution.

**Programming Language:** Python 3.10
**Framework:** RASA 3.0
**Frontend:** React JS with Tailwind CSS
**Backend:** Python (RASA action server)
**Tools:** IntelliJ IDEA, Pandas, Materialize CSS
**OS:** Windows 10
**Datasets:** Kaggle and Reddit (for mental health-related conversations)


**System Architecture**

The chatbot system includes the following major components:

**User Interface (Frontend):**
Built using React JS and Tailwind CSS, providing a responsive and calming web interface where users interact with the chatbot.

**RASA Backend:**

**RASA NLU (Natural Language Understanding):**
Processes user input, identifies intents (like “stress,” “depression,” or “exam pressure”), and extracts entities (like “English” or “Tamil” for communication preference).

**RASA Core (Dialogue Management):**
Handles multi-turn conversations using policies such as TEDPolicy, RulePolicy, and MemoizationPolicy to decide the next best action.

**Action Server:**
Executes custom Python code for specific actions like recommending a doctor based on user preferences (language, experience, consultation fee).

**Database Layer:**
A local dataset (doctor_appointment.xlsx) storing doctor details such as language, experience, consultation fee, and appointment links.

**Integration:**
The chatbot communicates between the user and backend using REST APIs (/webhooks/rest/webhook).



