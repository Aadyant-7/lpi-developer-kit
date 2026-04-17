# How I Did It – Level 2 (Khushi Garg)

## Step 1: Cloned the Repository
I cloned the LPI Developer Kit repository to my local system using:
git clone https://github.com/g-khushi/lpi-developer-kit.git

Then I navigated into the project folder:
cd lpi-developer-kit

---

## Step 2: Installed Dependencies
I installed all required packages using:
npm install

This step downloaded and configured all necessary dependencies for the project.

---

## Step 3: Built the Project
I built the project using:
npm run build

This step ensured that the project was properly compiled and ready to run.

---

## Step 4: Ran the Test Client
I executed:
npm run test-client

This command tested the working of the AI agent and connected tools.

---

## Step 5: Verified Tool Outputs
After running the test client, I verified that all tools were working correctly.  
The output showed:

[PASS] smile_overview  
[PASS] query_knowledge  
[PASS] get_case_studies  
[PASS] get_insights  
[PASS] list_topics  
[PASS] smile_phase_detail  
[PASS] get_methodology_step  

This confirmed that all 7 tools executed successfully.

---

## Step 6: AI Model Setup
I set up a local AI model using Ollama and used the LLaMA3 model.  
This allowed me to run AI responses locally without relying on external APIs.

---

## Step 7: LLM Output Verification
The model successfully generated responses explaining digital twin concepts using SMILE methodology.  
This confirmed that the AI model was working correctly with the system.

---

## Step 8: Understanding the Workflow
Through this process, I understood how:
- The test client interacts with different tools  
- AI agents use these tools to generate meaningful responses  
- SMILE methodology helps structure outputs clearly  

---

## Conclusion
By following these steps, I successfully set up the LPI Developer Kit on my system and verified that all tools and the AI model are working correctly.  
This completes my Level 2 implementation.
