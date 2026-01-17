# Hybrid AI Story Generator
Vision (BLIP) + Language (Mistral-7B)

# Problem Definition & Objective

## Problem Statement

Creative storytelling using AI often lacks contextual grounding when relying only on text or only on images. Traditional text-only models fail to capture visual emotions, while vision-only models cannot generate deep narratives.

## Objective

### To design a Hybrid AI Story Generator that

1. Understands visual input (images)
2. Interprets user intent from text
3. Generates coherent cinematic stories
4. Uses multi-modal intelligence combining Vision + Language models

## Real-World Motivation

### This system can be applied to:
1. AI storytelling & content creation
2. Game narrative generation
3. Creative writing assistants
4. AI-assisted filmmaking
5. Digital art and storytelling tools

## Selected Project Track

Hybrid AI System
(Computer Vision + Large Language Models)

# Data Understanding & Preparation

## Dataset Source
1. **Image Input:** User-provided images (real-world images)
2. **Text Input:** User-provided natural language prompts
3. **No fixed dataset** required (dynamic inference-based system)

## Data Processing

Images processed using BLIP Image Captioning
Text prompts parsed using keyword extraction

### Scene attributes inferred:

1. Mood
2. Weather
3. Time
4. Emotion
5. Narrative tone

## Preprocessing Steps

1. Image normalization using BLIP processor
2. Tokenization using Mistral tokenizer
3. Prompt structuring using instruction-tuned format
4. No missing data (real-time inputs)

# Model / System Design

## AI Techniques Used

**Computer Vision → BLIP (Vision-to-Text)**
**Large Language Model → Mistral-7B (4-bit quantized)**
**Prompt Engineering**
**Hybrid Pipeline Design**


## Architecture Overview

User Input  
    ↓  
Text Prompt  
    ↓  
Intent Analyzer  
    ↓  
Image → BLIP → Scene Understanding  
    ↓  
Context Builder  
    ↓  
Mistral-7B  
    ↓  
Cinematic Story Output



# Why This Design?
BLIP provides visual grounding
Mistral offers strong narrative generation
Quantization allows GPU-efficient execution
Modular design allows easy upgrades

# Core Implementation

## Key Components

1. BLIPProcessor → Image captioning
2. Mistral-7B Instruct → Story generation
3. BitsAndBytes → 4-bit quantization
### Custom pipeline for:
1. Intent detection
2. Context fusion
3. Prompt engineering
## Prompt Engineering Strategy
1. System instruction-based prompting
### Enforced story structure:
1. Conflict
2. Climax
3. Resolution
4. Style control (cinematic, poetic, emotional)
## Execution Flow
1. User enters text + optional image
2. Image captioned via BLIP
3. Context synthesized
4. Structured prompt created
5. Story generated via Mistral
6. Clean output returned

# Evaluation & Analysis
## Evaluation Type
1. Qualitative Evaluation
2. Human-centered evaluation
## Metrics Used
1. Narrative coherence
2. Visual relevance
3. Emotional consistency
4. Prompt adherence
Creativity score (manual)
## Sample Output
1. Emotion-aware storytelling
2. Scene continuity
3. Logical progression
Visual grounding from image
## Observed Limitations
1. No factual verification
2. Output varies with prompt clarity
3. Requires GPU for smooth execution

# Ethical Considerations & Responsible AI

## Bias & Fairness

1. Model may reflect biases from training data
2. Emotional interpretation may vary
3. No harmful intent filtering (can be added)

## Responsible Usage

1. No medical/legal decision-making
2. Intended for creative purposes only
3. User-controlled inputs prevent misuse

## Dataset Limitations

1. BLIP trained on generic image-caption datasets
2. Mistral trained on large-scale internet text

# Conclusion & Future Scope

## Summary

1. Successfully built a Hybrid Vision + Language AI
2. Achieved coherent, cinematic storytelling
3. Modular, scalable, and efficient design

## Future Improvements

1. Add speech-to-text input
2. Integrate diffusion-based image generation
3. Add emotion classifier
4. Support multi-character narratives
5. Deploy as a web app or API
