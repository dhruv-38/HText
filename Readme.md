# Handwritten Text Recognition AI Agent

## Author Information
**Name:** [Dhruv Choudhary]  
**University:** [IIT GN]  
**Department:** [Chemical Engineering]

## Project Overview

This project implements an AI agent that automates the manual task of **handwritten text recognition and transcription**. The agent uses a fine-tuned TrOCR (Transformers for Optical Character Recognition) model to automatically convert handwritten text images into digital text, eliminating the need for manual transcription.

### Manual Task Being Automated
- **Task:** Converting handwritten documents and forms into digital text
- **Current Manual Process:** Reading handwritten text and manually typing it into digital format
- **Time Consumption:** Hours of manual labor for large document sets
- **Error Prone:** Human transcription errors and fatigue-related mistakes
- **AI Solution:** Automated OCR with specialized handwriting recognition capabilities

## Technical Architecture

### Core Components

1. **Vision Encoder:** Processes handwritten images and extracts visual features
2. **Text Decoder:** Generates text sequences from visual representations
3. **LoRA Fine-tuning:** Parameter-efficient adaptation for handwriting recognition
4. **Evaluation System:** Metrics-based quality assessment

### Model Architecture
- **Base Model:** `microsoft/trocr-base-handwritten`
- **Framework:** Hugging Face Transformers + PEFT
- **Fine-tuning Method:** LoRA (Low-Rank Adaptation)
- **Dataset:** IAM Handwritten Forms Dataset

## Fine-tuning Strategy

### Why LoRA Fine-tuning?
- **Task Specialization:** Adapts the pre-trained TrOCR model for specific handwriting styles and document formats
- **Improved Reliability:** Reduces hallucinations and improves accuracy on domain-specific handwritten text
- **Resource Efficiency:** Only 0.45% of parameters are trainable, making it computationally efficient
- **Adapted Style:** Better recognition of cursive writing and form-specific layouts
