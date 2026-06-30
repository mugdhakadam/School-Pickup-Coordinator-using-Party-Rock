# School-Pickup-Coordinator-using-Party-Rock
Demonstration for quick Prototyping an Idea on everyday activity of a Mom

# Public Project Link:
https://partyrock.aws/u/MugdhaKadam/vMxMpl_3b/Neighborhood-School-Pickup-Coordinator-App


# Intent of building this App
As a parent, School pick and drop off of my child is a major responsiblity of the day. At the same time, considering today's job duties, we may or may not be present for the pick up. 
Hence, I got an idea why not create an  App for the same. I can utilise my friends/trusted sources in my neighbourhood and send a daily report of who needs to pick up the children from school and bring them safely to their homes. 

# Project Overview
Neighborhood School Pickup Coordinator App - An AI-powered coordination tool designed to help parents and neighbors efficiently organize school pickup duties through shared responsibility.

## Project Objectives
Streamline Communication: Enable parents to clearly communicate their availability and pickup commitments
Build Community Trust: Facilitate safe child pickup arrangements between trusted neighbors
Reduce Coordination Overhead: Automate the creation of pickup summaries to eliminate back-and-forth messaging
Enhance Safety: Maintain clear records of authorized adults for each child
Flexibility: Support varying schedules with multiple time slots and availability options

## Architecture
### Input Layer
Parent Information Inputs: Collects parent and child names
Availability Controls: Dropdown selectors for availability status and time preferences
Child-Specific Pickup Time: Dedicated selector for when the child needs pickup
Coordination Lists: Text inputs for neighbor children and trusted parents (with optional flag for flexibility)
### Processing Layer
AI-Powered Summary Generation: Uses Amazon Bedrock's Claude 4.6 Sonnet model to synthesize inputs into coherent, actionable summaries
Prompt Engineering: Structured prompt ensures consistent, friendly, well-formatted output
### Output Layer
Pickup Coordination Summary: Generated text output providing at-a-glance pickup information


## Underlying Technology
### Platform
PartyRock: Amazon's AI app building playground built on Amazon Bedrock
Amazon Bedrock: Managed service providing access to foundation models
### AI Model
Claude 4.6 Sonnet (bedrock-anthropic.claude-4-6-sonnet-v1-0)
Temperature: 0 (deterministic output for consistency)
### Widget Types Utilized
Static Text: Information display and project documentation
Text Input: Free-form data collection for names and lists
Select Dropdown: Structured choice inputs for availability and time slots
Inferred Text (AI Output): LLM-powered summary generation
### Design Principles
User-Centric Design: Simple, intuitive interface for busy parents
Optional Inputs: Flexibility for varying use cases
Structured Prompting: Ensures reliable, formatted AI outputs
Privacy-First: Local coordination without external API dependencies
