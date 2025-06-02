+++
title = "FormLoop"
date = "2025-05-31"
tags = ["project", "web", "react", "python", "gcp"]
draft = true
+++

**Automating recurring form signups with intelligent scheduling, eliminating the tedious weekly routine of manually sending Google Forms and managing waitlists for sports drop-ins.**

## Links
- **[🌐 Live Site](https://form-loop.vercel.app/)**
- **[💻 GitHub Repository](https://github.com/daniel-yili-ye/FormLoop)**

## Introduction

I help coordinate weekly sports drop-ins at my church. The process is typically the same week to week. Every week at a specific time, an admin needs to remember to send out a Google Form in a WhatsApp groupchat and a corresponding Google Sheet is shared to the group showing who signed up and who's on the waitlist. Complexity arises since we run multiple sports (basketball and volleyball) and admins and need to manage the signup wailist and user preferences for each sport / session they are responsible for on an ongoing basis.

After months of this tedious weekly ritual, I realized this was the perfect opportunity to build a solution that could automate the entire process while giving participants a better experience.

## The Problem

Managing recurring sports signups manually creates unnecessary overhead and potential for human error:

**Administrative burden:**
- Manually sending forms at scheduled times every week
- Sharing separate spreadsheets to show signup status and waitlists
- Managing the waitlist status over time as participants signup / dropout over time
- Remembering to open and close signups at the right times
- **Complexity specific to us:** Our volleyball drop-in runs two sessions every Wednesday night, and participants need to specify their session preference priority, something that's clunky for admins to manually handle with standard Google Forms / Sheets.

**User experience issues:**
- Participants have to wait for forms to be manually sent out
- No truly accurate real-time visibility into signup status or waitlist position
- No automated notifications about signup status (i.e. getting off the waitlist)

## The Solution

FormLoop is a web-based platform that automates the entire recurring signup workflow:

1. **Admin Setup**: Create forms for different activities with custom fields and capacity limits
   - Set specific requirements (like session preferences for volleyball)
   - Configure automatic scheduling for when signups open and close
   - Define waitlist behavior and notification preferences

2. **Automated Scheduling**: Forms automatically open and close based on your schedule
   - No more manual form sending every week
   - Participants know exactly when signups will be available
   - Consistent timing eliminates confusion

3. **Real-time Management**: Live updates for both admins and participants
   - Participants can see current signup status and waitlist position
   - Admins can edit signup lists and manage users on the fly
   - Automatic waitlist promotion when spots open up

4. **Multi-Activity Support**: Purpose-built to handle different sports with unique requirements
   - Basketball: Simple signup with capacity limits
   - Volleyball: Dual session preferences with priority ranking
   - Easily expandable to other activities with different needs

## Technology Stack

Built with reliable, well-tested technologies for consistent performance:

- **Frontend**: React for responsive user interfaces
- **Backend**: Flask (Python) for robust server-side logic
- **Database**: Firebase for real-time data synchronization
- **Scheduling**: Automated job scheduling for form management

## Impact & Future Plans

FormLoop is currently being developed to serve our church's basketball and volleyball drop-ins, with the possibility to expand to other recurring activities. The goal is to eliminate the weekly administrative overhead while providing participants with a better, more transparent signup experience.

**Planned improvements:**
- Admin analytics dashboard for tracking participation trends
- Support for payment collection for paid signup activities
- Multi-organization support for other churches or community groups

## Key Learnings

This project is providing valuable experience in:

- **Automation Design**: Building systems that reduce manual administrative tasks
- **Real-time Applications**: Implementing live updates with Firebase
- **User Experience**: Designing intuitive interfaces for both admins and participants
- **Scheduling Systems**: Creating reliable automated workflows for recurring events
- **Community Solutions**: Solving real problems for local organizations and volunteer coordinators