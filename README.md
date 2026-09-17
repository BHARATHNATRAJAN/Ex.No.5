# EXP 5: Comparing Prompting Techniques Through Engineering Problem-Solving Scenarios

## AIM

To compare different prompting techniques and evaluate their effectiveness in solving a real-world engineering problem by using a problem selected from a 3rd-year or final-year engineering project.

## AI TOOLS REQUIRED

* ChatGPT

## EXPERIMENT OVERVIEW

In this experiment, a real-world engineering problem is selected from a final-year project. The same problem is given to ChatGPT using different prompting techniques. The generated responses are compared based on quality, accuracy, depth, clarity, completeness, feasibility and usefulness.

The objective is to understand how prompt structure and clarity affect the quality of AI-generated solutions.

---

# STEP 1 – SELECT THE ENGINEERING PROBLEM

## Project Title

**Real-Time Personal Safety Application Using AI and Smartphone Sensors**

## Problem Statement

People travelling alone may face emergency situations where they are unable to manually press an SOS button or make a phone call. The proposed application detects unusual activities such as sudden running, prolonged inactivity and route deviation using smartphone sensors and GPS. When a possible emergency is detected, the system can notify trusted contacts along with the user's location.

---

# STEP 2 – SELECTED ENGINEERING SCENARIO

**Scenario:**

Design a mobile-based personal safety application that detects abnormal movement and route deviation using GPS, accelerometer and gyroscope data and provides an emergency alert mechanism.

---

# STEP 3 – BASE / NAÏVE PROMPT

### Prompt

"Create a personal safety app that detects danger and sends an SOS alert."

### AI-Generated Output

ChatGPT suggests creating a mobile safety application with an SOS button, GPS tracking, emergency contacts and automatic alerts. The application can detect unusual activities and send the user's location to trusted contacts.

### Observation

The response provides a general idea but does not give sufficient technical details about sensors, detection algorithms, implementation or testing.

---

# STEP 4 – DIFFERENT PROMPTING TECHNIQUES

## Technique 1 – Role-Based Prompting

### Prompt

"Act as an IoT and mobile application engineer. Design a real-time personal safety application using GPS, accelerometer and gyroscope sensors. The system should detect sudden running, prolonged inactivity and route deviation. Explain the system architecture, detection method, alert mechanism, technologies and testing procedure."

### AI-Generated Output

The AI provides a technical solution containing:

* GPS for location tracking
* Accelerometer and gyroscope for movement detection
* Activity classification
* Route monitoring
* Emergency alert generation
* Mobile application development
* Testing procedures

### Observation

Role-based prompting makes the response more technically focused and relevant to the engineering problem.

---

## Technique 2 – Step-by-Step Prompting

### Prompt

"Design the personal safety application step by step. First identify the requirements, then select suitable sensors, explain data collection, explain abnormal activity detection, describe GPS tracking, explain emergency alert generation and finally describe the testing procedure."

### AI-Generated Output

The solution is divided into:

1. Requirement identification
2. Sensor selection
3. Data collection
4. Data processing
5. Abnormal activity detection
6. GPS tracking
7. Emergency alert generation
8. System testing

### Observation

Step-by-step prompting produces a well-organized and easy-to-follow solution.

---

## Technique 3 – Few-Shot Prompting

### Prompt

"Use these examples to understand the required system behaviour:

Example 1: Normal walking → No emergency alert.

Example 2: Sudden unusual movement followed by prolonged inactivity → Safety verification.

Example 3: Significant route deviation → Check the user's safety.

Based on these examples, design a personal safety application using GPS, accelerometer and gyroscope data. Explain the detection logic and alert mechanism."

### AI-Generated Output

The AI maps different activities to suitable system actions.

| Activity                     | System Response     |
| ---------------------------- | ------------------- |
| Normal walking               | Continue monitoring |
| Sudden unusual movement      | Monitor activity    |
| Prolonged inactivity         | Safety verification |
| Route deviation              | Check user safety   |
| Multiple abnormal conditions | Emergency procedure |

### Observation

Few-shot prompting helps the AI understand the expected relationship between situations and system responses.

---

## Technique 4 – Constraint-Based Prompting

### Prompt

"Design a real-time personal safety mobile application with the following constraints: use GPS, accelerometer and gyroscope; operate in the background; detect sudden running, prolonged inactivity and route deviation; reduce false alerts; send the user's location to trusted contacts during an emergency; provide a simple implementation suitable for an engineering project; and explain the architecture, algorithm, limitations and testing procedure."

### AI-Generated Output

The AI provides a project-oriented solution that considers:

* Sensor requirements
* Background monitoring
* Activity detection
* GPS tracking
* Emergency notification
* False-alert reduction
* System limitations
* Testing and validation

### Observation

Constraint-based prompting gives a more practical and feasible solution because the project requirements are clearly specified.

---

# STEP 5 – COMPARISON / EVALUATION TABLE

| Prompting Technique     | Quality   | Accuracy | Depth     | Clarity   | Feasibility | Usefulness |
| ----------------------- | --------- | -------- | --------- | --------- | ----------- | ---------- |
| Naïve Prompt            | Medium    | Medium   | Low       | Medium    | Medium      | Medium     |
| Role-Based Prompt       | High      | High     | High      | High      | High        | High       |
| Step-by-Step Prompt     | High      | High     | High      | Very High | High        | Very High  |
| Few-Shot Prompt         | High      | High     | Medium    | High      | High        | High       |
| Constraint-Based Prompt | Very High | High     | Very High | High      | Very High   | Very High  |

---

# STEP 6 – ANALYSIS AND OBSERVATIONS

### Quality

The naïve prompt provides only a general solution. Improved prompts provide more detailed and project-specific information.

### Accuracy

Including technical requirements such as GPS, accelerometer and gyroscope helps ChatGPT focus on relevant engineering components.

### Depth

Step-by-step and constraint-based prompts provide deeper explanations of system architecture, algorithms, implementation and testing.

### Clarity

Step-by-step prompting produces information in a logical sequence, making it easier to understand.

### Feasibility

Constraint-based prompting makes the solution more practical by considering background operation, false alerts and emergency communication.

### Usefulness

Improved prompts are more useful for engineering projects because they provide implementation-oriented information.

### Does ChatGPT always provide better results with improved prompts?

No. A naïve prompt can be sufficient when the problem is simple and only a general answer is required. However, for complex engineering problems, structured prompts generally produce more relevant and detailed responses.

---

# STEP 7 – FINAL SELECTED PROMPTING TECHNIQUE

**Selected Technique: Constraint-Based Prompting combined with Step-by-Step Prompting**

This combination was selected because the engineering problem contains several technical requirements and practical constraints.

---

# STEP 8 – REFINED / FINAL PROMPT

"Act as an experienced IoT and mobile application engineer. Design a real-time personal safety mobile application for people travelling alone. The application must use smartphone GPS, accelerometer and gyroscope data to identify abnormal situations such as sudden running, prolonged inactivity and significant route deviation.

Explain the solution step by step, including:

1. Problem requirements
2. System architecture
3. Sensors and technologies required
4. Data collection and preprocessing
5. Activity detection algorithm
6. Emergency decision logic
7. GPS location tracking
8. Trusted-contact alert mechanism
9. Mobile application implementation
10. Testing and validation
11. False-alert reduction methods
12. Limitations and future improvements

Keep the solution technically realistic, beginner-friendly and suitable for a final-year engineering project."

---

# STEP 9 – ENGINEERING VALIDATION

The proposed system can be validated using different test cases.

| Test Case                    | Expected Result                 |
| ---------------------------- | ------------------------------- |
| Normal walking               | No emergency alert              |
| Normal running               | Continue monitoring             |
| Sudden unusual movement      | Detect abnormal activity        |
| Prolonged inactivity         | Initiate safety verification    |
| Route deviation              | Detect deviation                |
| Multiple abnormal conditions | Trigger emergency procedure     |
| GPS unavailable              | Provide suitable fallback/error |
| False detection              | Verify false-alert reduction    |

The system can be evaluated using:

* Detection accuracy
* False-positive rate
* False-negative rate
* Alert delivery time
* GPS accuracy
* Battery consumption
* System response time

---

# CONCLUSION

Different prompting techniques produce different levels of quality in AI-generated engineering solutions. The naïve prompt provides a basic response, whereas role-based, step-by-step, few-shot and constraint-based prompts provide more structured and technically relevant solutions.

For complex engineering problems, combining **step-by-step prompting and constraint-based prompting** provides a detailed, feasible and useful solution.

# RESULT

**The prompt for the above-mentioned engineering problem was executed successfully, and the responses generated using different prompting techniques were compared and evaluated based on quality, accuracy, depth, clarity, feasibility and usefulness.**
