# AI Document Analyzer
A lightweight, single-file web application that leverages the Google Gemini API to instantly summarize, extract key points, and calculate metrics from text documents.

## Features
Instant Summarization: Generate brief, standard, or detailed summaries of your text.

Key Insights: Automatically extracts up to 5 critical points from the document.

Document Metrics: Calculates word count, sentence count, estimated reading time, tone, complexity, and detected language.

Flexible Input: Paste raw text directly or upload a file via drag-and-drop (.txt, .md, .csv up to 50 KB).

Modern UI: Clean, responsive tabbed interface built with vanilla HTML/CSS and Tabler Icons.

Structured Output: Uses Gemini's JSON schema generation capabilities to ensure reliable, cleanly formatted results.

## Prerequisites
To run this application, you will need a Google Gemini API Key. You can obtain one from Google AI Studio.

## Getting Started
Download the file: Save the provided code as an .html file (e.g., index.html).

## Add your API Key: Open the file in your preferred code editor and locate the configuration section near the top of the <script> tag. Replace the placeholder string with your actual API key:

## JavaScript
// --- CONFIGURATION ---
const GEMINI_API_KEY = 'YOUR_API_KEY_HERE'; 
Run the app: Simply double-click the .html file to open it in your web browser. No local server, package managers, or build tools are required.

## Usage
Open the application in your browser.

Paste your text into the text area OR drag and drop a supported file into the upload zone.

Select your preferred Summary Length from the dropdown menu (Brief, Standard, or Detailed).

Click Analyze Text.

Navigate between the Summary, Key Points, and Metrics tabs to view the AI-generated results.

Use the Copy button to quickly copy the active summary to your clipboard.

## Technologies Used
Frontend: HTML5, CSS3 (Custom Variables, Flexbox/Grid), Vanilla JavaScript

Icons: Tabler Icons (via CDN)

Fonts: Inter and JetBrains Mono (via Google Fonts)

AI Integration: Google Gemini API (gemini-2.5-flash model via REST/Fetch API)

## ⚠️ Security Warning for Production Deployment
This application is designed as a client-side-only, single-file tool. Hardcoding your API key in the frontend JavaScript is suitable for local testing and personal use only. If you plan to deploy this application to the public web (e.g., on GitHub Pages, Vercel, or Netlify), anyone inspecting the page source can steal your API key. For public deployment, you must move the API call to a backend server or a serverless function to keep your API key secure.
