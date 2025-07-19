# Resume_Checker
🔍 Purpose
To check ATS (Applicant Tracking System) compatibility by analyzing a resume and matching it against required skills from a job description, providing insights and suggestions for improvement.

🛠️ Key Functionalities
Skill Matching:

Uses pre-defined skill sets for common job roles like AI/ML Intern, Data Analyst, Web Developer, etc.

Compares extracted resume skills against these roles to determine the best fit.

Resume Text Extraction:

Converts PDF resume to images using pdf2image.

Extracts text using pytesseract (OCR).

JD Keyword Extraction:

Tokenizes and cleans the job description text using nltk.

Removes stopwords and keeps only meaningful keywords.

ATS Score Calculation:

Compares found skills against a pool of total skills to calculate a percentage match.

Generates a pie chart visualizing the match percentage.

Feedback Generation:

Provides actionable suggestions based on the ATS score.

Suggests best-fit job roles and secondary options.

🖼️ User Interface (Gradio):
Inputs:

Resume file (PDF).

Job Description (text input).

Outputs:

Pie chart of ATS score.

Markdown text with suggestions and recommended roles.

📦 Dependencies Used
gradio (for UI)

pdf2image, pytesseract (for PDF & OCR)

nltk (for keyword extraction)

matplotlib (for pie chart)

PyMuPDF (fitz) and PIL (for image/PDF handling)

🌐 Deployment
Designed to launch via demo.launch(share=True), which makes it accessible via a public Gradio URL.

✅ Summary
This is an AI-powered resume screening tool that mimics how recruiters or ATS systems evaluate resumes. It is ideal for:

Job seekers refining their resumes.

Career counselors.

Developers building smart hiring platforms.

