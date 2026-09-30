# Meeting Transcript Summariser

Generative AI capstone project that converts a plain-text meeting transcript into a structured meeting summary, decisions, action items, and downloadable reports.

## Current implementation
- Google Colab
- Groq API with Llama 3.3 70B
- Python `json` parsing
- pandas for action-item tables
- ReportLab for PDF generation
- Input: `.txt` meeting transcript
- Output: structured summary, `meeting_summary.txt`, and `Meeting_Report.pdf`

## Repository structure

```text
meeting-transcript-summariser/
├── Project_9_Meeting_Transcript_Summariser.ipynb   # upload your actual Colab notebook here
├── sample_transcripts/
│   ├── Sample1Transcript.txt                       # add your actual tested file
│   ├── Sample2Transcript.txt                       # add your actual tested file
│   └── Sample3Transcript.txt
├── outputs/
│   └── Meeting_Report_Sample3.pdf
├── reports/
│   └── Meeting_Transcript_Summariser_Report_UPDATED.docx
├── .gitignore
├── requirements.txt
└── README.md
```

## How to upload the actual project

1. Open the GitHub repository.
2. Upload the `.ipynb` notebook used for the final project.
3. Upload the three transcript files used for testing.
4. Upload the final generated PDF and the updated project report if required by the submission.
5. Do **not** upload API keys, `.env` files, Colab secrets, or any private credentials.
6. Commit the changes with a message such as `Add final meeting transcript summariser project`.

## API key safety

Store the Groq API key in Google Colab Secrets or an environment variable. Never hard-code the key in the notebook or commit it to GitHub.

## Testing evidence

The supplied Sample 3 transcript is included in `sample_transcripts/Sample3Transcript.txt`. Its generated output identifies the meeting as a Review, records the decision to hire two support engineers, and extracts three action items with owners and deadlines.

The other two transcript files should be added using the exact files actually tested. Do not replace them with invented examples if the report is intended to document real test runs.

## Suggested GitHub repository contents

At minimum, upload:
- final `.ipynb`
- three tested `.txt` transcripts
- `README.md`
- optional `requirements.txt`
- final generated PDF
- project report, if your submission requires it

## Important

The current package does not invent the missing notebook or the other two transcript files because they were not supplied with this upload.
