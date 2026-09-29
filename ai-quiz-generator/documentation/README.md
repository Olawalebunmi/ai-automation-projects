AI Quiz Generator & Multi-Channel Notification Automation

An AI-powered quiz generation and notification workflow built with Make.com, Google Sheets, Google Gemini, Gmail, and Telegram.

The automation monitors a Google Sheet for new quiz requests, uses Google Gemini to generate quiz content, routes requests according to their learning track, and delivers the result through email and Telegram.


Project Overview

Creating and distributing customized quizzes manually can be repetitive and time-consuming.

This project demonstrates how AI and workflow automation can be combined to streamline quiz generation and distribution.

The workflow connects:

- Google Sheets — structured input and data source
- Google Gemini — AI-powered quiz generation
- Make.com Router — conditional workflow routing
- Gmail — email delivery
- Telegram — real-time notification

The result is an end-to-end automation that transforms a structured quiz request into AI-generated educational content and distributes it through multiple channels.


Objectives

The automation was designed to:

1. Capture quiz requests from Google Sheets.
2. Pass structured information to Google Gemini.
3. Generate quiz content using an AI model.
4. Route requests based on learning track.
5. Send the generated content by email.
6. Send a Telegram notification.
7. Support multiple workflow paths.
8. Provide a structure that can be extended with additional automation and error handling.


Workflow Architecture

                    ┌─────────────────────┐
                    │    Google Sheets    │
                    │   Watch New Rows    │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    Google Gemini    │
                    │   Generate Quiz     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │       Router        │
                    │  Conditional Logic  │
                    └───────┬───┬───┬─────┘
                            │   │   │
                ┌───────────┘   │   └───────────┐
                ▼               ▼               ▼
        ┌─────────────┐ ┌─────────────┐ ┌─────────────┐
        │   Advanced  │ │  Practical  │ │ Foundation  │
        │    Track    │ │    Track    │ │    Track    │
        └──────┬──────┘ └──────┬──────┘ └──────┬──────┘
               │               │               │
               ▼               ▼               ▼
           ┌───────┐       ┌───────┐       ┌───────┐
           │ Gmail │       │ Gmail │       │ Gmail │
           └───┬───┘       └───┬───┘       └───┬───┘
               │               │               │
               ▼               ▼               ▼
           Telegram         Telegram         Telegram